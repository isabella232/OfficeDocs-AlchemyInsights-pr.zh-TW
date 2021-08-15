---
title: 在 Microsoft 365 應用程式中登入的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: b0789a54f48b2850c1dad8651a8209449c805784bea96799f05e67c4bc43fdb0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53986882"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>修正 Microsoft 365 的應用程式「您電腦的信任的平臺模組無法正常運作」訊息

若要修正此錯誤，請嘗試下列步驟：

- 為[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)安裝最新的更新。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。  (Ex： \Software\Microsoft\ Office \16.0\Common\Identity\)
- 嘗試 [使用者](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 復原程式以修正受信任的平臺模組 (TPM) 失敗。
- 使用下列步驟設定 EnableADAL = 0：  
    1. 以滑鼠右鍵按一下 Windows [開始] 按鈕，選擇 [**執行**]，輸入 **regedit**，然後選擇 **[確定]**。
    2. 選取 **[是]** 以允許登錄編輯程式對您的裝置進行變更。
    3. 在 [登錄編輯程式] 中，在 [HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity] 下新增 **EnableADAL** 的 DWORD 值，設定為 **0** 。

如需詳細資訊，請參閱[update to Office 2016 build 16.0.7967 on on Windows 10 上的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。