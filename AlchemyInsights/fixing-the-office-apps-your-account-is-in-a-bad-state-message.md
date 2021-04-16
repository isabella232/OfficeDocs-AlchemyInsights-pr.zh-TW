---
title: 修正 Microsoft 365 應用程式您的帳戶處於不良的狀態訊息
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
- "2558"
- "9000571"
ms.openlocfilehash: 4654b49289a455c1e6641f47fae573d2fcebc717
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812527"
---
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a>修正 Microsoft 365 應用程式「您的帳戶處於不良狀態」錯誤

若要修正此錯誤，請在受影響的電腦上嘗試下列選項：

- 開啟 Office 應用程式，選取 [**檔**  >  **帳戶**  >  **登出所有帳戶**]。 使用具有有效授權的使用者帳戶再次登入。 如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br>
  **附注：** Office 2016 的登錄路徑已變更為16.0。 例如，\Software\Microsoft\Office\16.0\Common\Identity\
- 如果使用 Office 2013 連線到 Office 365 時發生錯誤，請啟用 Office 用戶端的 [新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 。

如需詳細資訊，請參閱 how [to 疑難排解無法登入 Microsoft 365、Azure 或 Intune 的非瀏覽器應用程式](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)。

