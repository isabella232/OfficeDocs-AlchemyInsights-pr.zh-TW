---
title: 登入 Microsoft 365 應用程式時的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709097"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a>修正 Microsoft 365 應用程式「您電腦的信任的平臺模組無法正常運作」訊息

若要修正此錯誤，請嘗試下列步驟：

- 安裝最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。  (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)
- 嘗試 [使用者](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) 復原程式以修正受信任的平臺模組 (TPM) 失敗。
- 使用下列步驟設定 EnableADAL = 0：  
    1. 以滑鼠右鍵按一下 [Windows 開始] 按鈕，選擇 [ **執行**]，輸入 **regedit**，然後選擇 **[確定]**。
    2. 選取 **[是]** 以允許登錄編輯程式對您的裝置進行變更。
    3. 在 [登錄編輯程式] 中，在 [HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity] 下新增 **EnableADAL** 的 DWORD 值，設定為 **0** 。

如需詳細資訊，請參閱在 [Windows 10 上更新到 Office 2016 build 16.0.7967 後，登入的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。