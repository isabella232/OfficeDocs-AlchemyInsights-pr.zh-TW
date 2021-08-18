---
title: 疑難排解 PRT 問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: a005c4a6848bbf0725560375df1220ce906cbb5f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330950"
---
# <a name="troubleshoot-prt-issue"></a>疑難排解 PRT 問題

若要讓任何裝置完成取得驗證，必須完全註冊且狀態良好，且能夠 (PRT) 取得主要重新整理權杖。

混合式 Azure AD join 註冊程式需要裝置在公司網路上。 它也會透過 VPN 運作，但有一些對該功能的忠告。 在遠端工作情況下，我們已聽說客戶需要協助疑難排解混合式 Azure AD join 註冊程式。 以下是在註冊過程中，出現在「蓋子」下的情況明細。

**使用 Azure AD 密碼雜湊同步處理或透過驗證的雲端驗證環境 ()**

此註冊流程也稱為「同步加入」。

1. Windows 10 使用者登入裝置時搜尋 SCP 記錄。
    1. 裝置會先嘗試從登錄中的用戶端 SCP 中取得租使用者資訊 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。 如需詳細資訊，請參閱本[文件](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    2. 若失敗，裝置會與內部部署 Active Directory (AD) 進行通訊，以從服務連線點 (SCP) 取得租使用者資訊。 若要驗證 SCP，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。 

**附注**：我們建議您在 AD 中啟用 SCP，且僅使用用戶端 SCP 進行初始驗證。

2. Windows 10 會嘗試與系統內容底下的 azure ad 進行通訊，以針對 Azure ad 進行自我驗證。 您可以使用 Test Device Registration Connectivity 腳本，確認裝置是否可以存取系統帳戶底下的 Microsoft 資源。

3. Windows 10 會產生自我簽署憑證，並將它儲存在內部部署 AD 中的 computer 物件底下。 這需要在網域控制站上進行直線。

4. 具有憑證的裝置物件會透過 Azure AD 連線同步處理至 Azure AD。 同步處理週期預設為每30分鐘，但其取決於 Azure AD 連線的設定。 如需詳細資訊，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此階段，您應該可以在 Azure 入口網站的裝置 blade 下，于「擱置」狀態看到主體裝置。

6. 在下一個使用者登入時 Windows 10，註冊將會完成。 

**附注**：如果您使用的是 VPN，且登出登入程式會終止網域連線，您可以手動觸發註冊：
 1. 在以系統管理提示或從 PSExec 遠端透過 PSExec 向您的電腦發出 dsregcmd/join。 例如，PsExec-s \\ win10client01 cmd，dsregcmd/join

 2. 如需混合式加入問題的詳細資訊，請參閱 [裝置問題疑難排解](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)。
