---
title: 我受到符合規範裝置的條件式存取封鎖
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 709749b1a62f2d9cdabfb3fe4b7538c22101d7109204d9163f6059336b817bf8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54019139"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>我受到符合規範裝置的條件式存取封鎖

**強烈建議的工具**

- [裝置註冊疑難排解員工具](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 完整的工具，可協助疑難排解最常見的裝置註冊問題。
- [測試裝置註冊連線能力指令碼](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 用來確保裝置可以存取系統帳戶下裝置註冊端點的工具。
- [Azure AD 裝置清理指令碼](https://github.com/mzmaili/AzureADDeviceCleanup) - 用來尋找和管理您環境中過時裝置的工具。

以下是條件式存取在符合規範的裝置上可能會失敗的原因，或為何在組織資源的登入要求期間，您的使用者可能會收到 **[您無法從這裡完成]** 的訊息。

1. **裝置不是使用 MDM 所需的裝置狀態**：

驗證裝置是否向核准的 MDM 提供者 (例如 Intune) 註冊，並 *標示為符合規範*。 如需有關 Intune 的詳細資訊，請參閱本[文件](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)。 若要深入瞭解裝置合規性和 Intune，請參閱[使用合規性原則為使用 Intune 管理的裝置設定規則](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)。 如果您在使用 Intune 註冊裝置時遇到問題，請參閱 [在 Microsoft 中對裝置註冊進行疑難排解](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) (部分機器翻譯) 上的疑難排解詳細資料。 若要進一步獲得 Intune 支援，請建立支援要求。 若要這樣做，請瀏覽 [Intune 的協助及支援頁面](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)。

2. **裝置未加入組織網路**：

若要存取組織資源，裝置必須透過直接連線或虛擬私人網路 (VPN) 連線到組織的網路，並且也加入內部部署或 Azure Active Directory。 若要將工作裝置加入組織網路，請參閱[將您的工作裝置加入組織的網路](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) (部分機器翻譯)。 若要註冊個人/BYOD 裝置，請參閱[在組織的網路上註冊您的個人裝置](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network) (部分機器翻譯)。

- 若要驗證裝置是否已加入網路，您可以按照[此處](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) (部分機器翻譯) 的步驟註冊裝置，或[此處](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) (部分機器翻譯) 的步驟註冊工作裝置。 若要將問題的範圍縮小為組織網路連線，請遵循下列指導方針：

    1. 使用工作或學校帳戶登入 Windows，例如 alain@contoso.com。
    2. 透過 VPN 或 DirectAccess 連線到貴組織的網路。
    3. 連線之後，請按 **Windows 標誌鍵+L** 鎖定您的裝置。
    4. 使用公司或學校帳戶解除鎖定您的裝置，然後再次嘗試存取有問題的應用程式或服務。

如果您再次看到 **[您無法從這裡完成]** 錯誤訊息，問題可能出在其他地方。

3. **不支援的作業系統**：

請確保您目前的作業系統版本受支援，包括：

- **Windows 用戶端**：Windows 7 或更新版本

- **Windows 伺服器**：Windows Server 2008 R2 或更新版本

- **macOS**：macOS X 或更新版本

- **Android 和 iOS**：最新版本的 Android 和 iOS 行動裝置作業系統

4. **不支援的網頁瀏覽器**：

請在下方尋找支援的瀏覽器。 對於 Windows 1703 或更新版本的 Chrome 支援，需要 Windows 10 帳戶擴充功能。 對於 Microsoft Edge 85+，使用者必須登入，以正確傳遞裝置合規性資訊。 如需詳細資訊，請參閱[此處](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support) (部分機器翻譯)。

- **Windows 10**：Microsoft Edge、Internet Explorer、Chrome
- **Windows 8 / 8.1**：Internet Explorer、Chrome
- **Windows 7**：Internet Explorer、Chrome
- **iOS**：Microsoft Edge、Intune Managed Browser、Safari
- **Android**：**Microsoft Edge**：Intune Managed Browser、Chrome
- **Windows Phone**：Microsoft Edge、Internet Explorer
- **Windows Server 2019**：Microsoft Edge、Internet Explorer、Chrome
- **Windows Server 2016**：Internet Explorer
- **Windows Server 2012 R2**：Internet Explorer
- **Windows Server 2008 R2**：Internet Explorer
- **macOS**：Chrome、Safari

在 [這裡](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation) (部分機器翻譯) 找到有關 **[您無法從這裡完成]** 的訊息和疑難排解步驟。
