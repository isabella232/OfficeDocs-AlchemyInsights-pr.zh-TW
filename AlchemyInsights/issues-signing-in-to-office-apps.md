---
title: 登入 Microsoft 365 應用程式時的問題
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
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579928"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>修正 Microsoft 365 應用程式 "對不起，您組織中的另一個帳戶已經登入" 郵件

若要修正此錯誤，請嘗試下列步驟：

- 移除所有工作帳戶（受影響的帳戶除外）使用 Windows 設定 >**存取工作或學校**。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。 （Ex： \Software\Microsoft\Office\16.0\Common\Identity\)
- 開啟 Office 應用程式 **，選擇 [** 檔案  >  **帳戶**] [登出]  >  ** **。然後使用具有有效授權的使用者帳戶登入。 如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 若是 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。

如需詳細資訊，請參閱[Office 中的「很抱歉，您組織中的另一個帳戶已登入這部電腦](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」。