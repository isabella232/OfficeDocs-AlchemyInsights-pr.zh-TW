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
# <a name="fixing-the-microsoft-365-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="c25dd-102">修正 Microsoft 365 應用程式「您的帳戶處於不良狀態」錯誤</span><span class="sxs-lookup"><span data-stu-id="c25dd-102">Fixing the Microsoft 365 apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="c25dd-103">若要修正此錯誤，請在受影響的電腦上嘗試下列選項：</span><span class="sxs-lookup"><span data-stu-id="c25dd-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="c25dd-104">開啟 Office 應用程式，選取 [**檔**  >  **帳戶**  >  **登出所有帳戶**]。</span><span class="sxs-lookup"><span data-stu-id="c25dd-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="c25dd-105">使用具有有效授權的使用者帳戶再次登入。</span><span class="sxs-lookup"><span data-stu-id="c25dd-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="c25dd-106">如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="c25dd-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="c25dd-107">使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="c25dd-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="c25dd-108">**附注：** Office 2016 的登錄路徑已變更為16.0。</span><span class="sxs-lookup"><span data-stu-id="c25dd-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="c25dd-109">例如，\Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="c25dd-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="c25dd-110">如果使用 Office 2013 連線到 Office 365 時發生錯誤，請啟用 Office 用戶端的 [新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) 。</span><span class="sxs-lookup"><span data-stu-id="c25dd-110">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="c25dd-111">如需詳細資訊，請參閱 how [to 疑難排解無法登入 Microsoft 365、Azure 或 Intune 的非瀏覽器應用程式](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1)。</span><span class="sxs-lookup"><span data-stu-id="c25dd-111">For more information, see [How to troubleshoot non-browser apps that can't sign in to Microsoft  365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

