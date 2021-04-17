---
title: 登入 Microsoft 365 應用程式時的問題
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
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833066"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="4364d-102">修正 Microsoft 365 應用程式 "對不起，您組織中的另一個帳戶已經登入" 郵件</span><span class="sxs-lookup"><span data-stu-id="4364d-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="4364d-103">若要修正此錯誤，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="4364d-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="4364d-104">移除所有工作帳戶（受影響的帳戶除外）使用 Windows 設定 > **存取工作或學校**。</span><span class="sxs-lookup"><span data-stu-id="4364d-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="4364d-105">使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="4364d-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="4364d-106">**附注：** Office 2016 的登錄路徑已變更為16.0。</span><span class="sxs-lookup"><span data-stu-id="4364d-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="4364d-107"> (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="4364d-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="4364d-108">開啟 Office 應用程式 **，選擇 [** 檔案  >  **帳戶**] [登出]  >  \*\*\*\*。然後使用具有有效授權的使用者帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="4364d-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="4364d-109">如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="4364d-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="4364d-110">若是 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。</span><span class="sxs-lookup"><span data-stu-id="4364d-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="4364d-111">如需詳細資訊，請參閱 [Office 中的「很抱歉，您組織中的另一個帳戶已登入這部電腦](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)」。</span><span class="sxs-lookup"><span data-stu-id="4364d-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>