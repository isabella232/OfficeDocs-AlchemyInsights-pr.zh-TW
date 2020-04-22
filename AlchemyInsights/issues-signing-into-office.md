---
title: 登入 Office 應用程式時的問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762968"
---
# <a name="issues-signing-in-to-office-apps"></a>登入 Office 應用程式時的問題

若要修正 Office 應用程式的登入問題，請嘗試下列步驟：

- 移除所有工作帳戶（受影響的帳戶除外）使用 Windows 設定 >**存取工作或學校**。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。 （Ex： \Software\Microsoft\Office\16.0\Common\Identity\)
- 開啟 Office 應用程式 **，選擇 [** > 檔案**帳戶** > ]**[登出]。** 然後使用具有有效授權的使用者帳戶登入。 如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 若是 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。
- 如果使用 Office 2013 連接至 Microsoft 365 時，發生錯誤，請啟用 Office 用戶端的新式驗證。

如需詳細資訊，請參閱：
- [您無法登入 Microsoft 365、Azure 或 Intune](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [在 Windows 10 上更新 Office 2016 build 16.0.7967 之後，登入後的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- ["很抱歉，您組織中的另一個帳戶已在這部電腦上登錄" （Office）](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [使用 ADFS 時疑難排解 Office 新式驗證的登入問題](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)