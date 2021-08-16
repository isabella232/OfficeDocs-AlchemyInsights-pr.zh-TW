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
- "2560"
ms.openlocfilehash: 454000eafa6818f91e3c302cc69fbf252aae1107aa18904ac93a4756d4db642b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028031"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a>修正 Microsoft 365 應用程式 "對不起，您組織中的另一個帳戶已經登入" 郵件

若要修正此錯誤，請嘗試下列步驟：

- 使用 Windows 設定 >**存取單位或學校**，移除所有的工作帳戶（受影響的帳戶除外）。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。  (Ex： \Software\Microsoft\ Office \16.0\Common\Identity\)
- 開啟 Office 應用程式 **，選擇 [** 檔案  >  **帳戶**] [登出]  >  ****。然後使用具有有效授權的使用者帳戶登入。 如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 若是 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。

如需詳細資訊，請參閱[Office 中的「很抱歉，您組織中的其他帳戶已登入此電腦](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」。