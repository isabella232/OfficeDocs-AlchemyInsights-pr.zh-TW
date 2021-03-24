---
title: 我因為已加入網域的裝置而受到條件式存取封鎖
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/20/2021
ms.locfileid: "50965460"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>我因為已加入網域的裝置而受到條件式存取封鎖

**強烈建議的工具**

[裝置註冊疑難排解員工具](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 此工具可協助排解最常見的裝置註冊疑難問題。

[測試裝置註冊連線能力指令碼](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 該指令碼有助於確保裝置可以存取系統帳戶下的裝置註冊端點。

[Azure AD 裝置清理指令碼](https://github.com/mzmaili/AzureADDeviceCleanup) - 該指令碼讓您能夠尋找和管理環境中過時的裝置。

以下是條件式存取在已加入網域 (混合式 Azure AD) 的裝置上可能失敗的一些常見原因。

1. **裝置上沒有 Azure AD PRT** - 您必須確保裝置具備 Azure AD 主要重新整理權杖 (PRT)。 如需有關 PRT 的詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)。

若要驗證您是否具備 Azure AD PRT，您可以在裝置上執行`dsregcmd/status`命令，並驗證「AzureAdPrt」是否等於「YES」。

如果「AzureAdPrt」是「NO」，請檢查下列項目：

- **您是否有具備 AD FS 的聯盟環境，而且無法從使用者家用網路進行連接**：在這種情況下，請確保您的「usernamemixed」端點可從外部網路進行存取。 如果您的 AD FS 位於 VPN 後面，請確保使用者連線至 VPN，然後重新登入裝置。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)。

- **裝置 TPM 是否故障，因而無法驗證裝置**：檢查「tpm.msc」以查看 TPM 的狀態是否「就緒」。 如果沒有，請執行 `dsregcmd/leave`，並讓裝置重新加入 Azure AD。 然後再試一次。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)。

- **您使用的是協力廠商身分識別提供者，該提供者不支援 WS-Trust 通訊協定**。 如我們的文件中的說明，已使用混合式 Azure AD 而聯結的裝置無法在此案例中使用。 請與身分識別提供者合作以取得支援。

2. **使用者使用 Chrome 瀏覽器時沒有 Windows 10 帳戶** 或 **Chrome 瀏覽器版的 Office 擴充功能不會自動在已加入 AAD 或已加入混合式 AAD 的裝置上使用 PRT**：這會導致任何以裝置為基礎的條件式存取原則失敗，並顯示「未註冊的裝置」錯誤訊息。 若要正確使用 Chrome 瀏覽器，您必須透過 SCCM 或 Intune 安裝「Windows 10 帳戶」或「使用者的 Chrome 瀏覽器的 Office 擴充功能」。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)。

如果無法從遠端推送延伸模組，請通知使用者手動安裝上述其中一個延伸模組，以存取裝置型條件式存取背後的應用程式。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)。

3. **裝置已正確使用混合式 Azure AD 而聯結，但因為 Azure AD Connect 或 Azure 入口網站中的同步處理變更而遭到意外刪除或停用**：如果發生這種情況，即使裝置上的「AzureAdJoined」和「PRT」狀態顯示為有效，裝置物件還是無法再識別為完全聯結的裝置。

若要修正此問題，請在受影響的裝置上執行 `dsregcmd/leave`，並讓它們重新加入 Azure AD。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)。

> [!NOTE]
> 如果您的裝置是使用 VPN/Cloud Proxy 的 Windows 10 1809 更新，且看到「AzureAdPrt」狀態或任何發生 SSO 問題的應用程式 (即使您有 PRT，Outlook 仍無法連線至信箱) 的問題，請確保您有此修補程式 [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) 或 4 月累積更新 [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6)，以防止這些機器上的 PRT 失敗。

















