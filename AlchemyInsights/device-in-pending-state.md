---
title: 處於擱置狀態的裝置
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53913994"
---
# <a name="device-in-pending-state"></a>處於擱置狀態的裝置

**先決條件：**

1. 如果您是第一次設定裝置註冊，請確定您已在[Azure Active Directory (azure ad) 中檢查過裝置管理簡介](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support)，以引導您瞭解如何在 azure ad 的控制下取得裝置。
2. 如果您直接向 Azure AD 註冊裝置，並將其註冊到 Intune，您必須確定您已 [設定 intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) 並且先進行 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) 。
3. 確定您有權在 Azure AD 和內部部署 AD 中執行作業。 只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。 此外，如果您要在 Windows Server Active Directory 中設定自動註冊，您必須是 Active Directory 和 AD FS 的系統管理員 (如果適用)。

混合式 Azure AD join 註冊程式需要裝置在公司網路上。 它也會透過 VPN 運作，但有一些對該功能的忠告。 我們聽說客戶在遠端工作情況下，需要協助疑難排解混合式 Azure AD join 註冊程式。

**使用 Azure AD 密碼雜湊同步處理或透過驗證的雲端驗證環境 ()**

此註冊流程也稱為「同步加入」。

以下是註冊程式期間所發生狀況的分解：

1. Windows 10 探索在使用者登入裝置時 (SCP) 記錄的服務連線點。

    1. 裝置會先嘗試從登錄中的用戶端 SCP 中取得租使用者資訊 [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]。 如需詳細資訊，請參閱 [document](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)。
    1. 如果失敗，裝置會與內部部署的 Active Directory 通訊，以取得來自 SCP 的承租人資訊。 若要驗證 SCP，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)。

    > [!NOTE]
    > 我們建議您在 Active Directory 中啟用 SCP，而且只能使用用戶端 SCP 進行初始驗證。

2. Windows 10 會嘗試與系統內容底下的 azure ad 進行通訊，以針對 Azure ad 進行自我驗證。

    您可以使用 [Test Device Registration Connectivity 腳本](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)，確認裝置是否可以存取系統帳戶底下的 Microsoft 資源。

3. Windows 10 會產生自我簽署憑證，並將它儲存在內部部署 Active Directory 中的 computer 物件底下。 這需要在網域控制站上進行直線。

4. 具有憑證的裝置物件會透過 Azure AD 連線同步處理至 Azure AD。 同步處理週期預設為每30分鐘，但是取決於 Azure AD 連線的設定。 如需詳細資訊，請參閱本 [檔](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)。

5. 在此階段，您應該可以在 Azure 入口網站的裝置 blade 下，于「**擱置**」狀態看到主體裝置。

6. 在下一個使用者登入時 Windows 10，註冊將會完成。

    > [!NOTE]
    > 如果您是在 VPN 上，且登出/登入已中斷網域連線，您可以手動觸發註冊。 若要執行這項作業，請完成下列程序：
    >
    > `dsregcmd /join`在本機上以系統管理員的身分，或透過 PSExec 從 PSExec 向您的電腦發佈。
    >
    > 例如：`PsExec -s \\win10client01 cmd, dsregcmd /join`

如 Azure Active Directory 裝置註冊的常見問題，請參閱[裝置常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq)。
