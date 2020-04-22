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
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="6908e-102">登入 Office 應用程式時的問題</span><span class="sxs-lookup"><span data-stu-id="6908e-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="6908e-103">若要修正 Office 應用程式的登入問題，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="6908e-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="6908e-104">移除所有工作帳戶（受影響的帳戶除外）使用 Windows 設定 >**存取工作或學校**。</span><span class="sxs-lookup"><span data-stu-id="6908e-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="6908e-105">使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。</span><span class="sxs-lookup"><span data-stu-id="6908e-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="6908e-106">**附注：** Office 2016 的登錄路徑已變更為16.0。</span><span class="sxs-lookup"><span data-stu-id="6908e-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="6908e-107">（Ex： \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="6908e-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="6908e-108">開啟 Office 應用程式 **，選擇 [** > 檔案**帳戶** > ]**[登出]。** 然後使用具有有效授權的使用者帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="6908e-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="6908e-109">如需詳細資訊，請參閱 [Office 的帳戶](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)。</span><span class="sxs-lookup"><span data-stu-id="6908e-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="6908e-110">若是 Mac，請參閱[無法登入 Mac 版 Office 2016 應用程式](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)。</span><span class="sxs-lookup"><span data-stu-id="6908e-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="6908e-111">如果使用 Office 2013 連接至 Microsoft 365 時，發生錯誤，請啟用 Office 用戶端的新式驗證。</span><span class="sxs-lookup"><span data-stu-id="6908e-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="6908e-112">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="6908e-112">For more information, see:</span></span>
- [<span data-ttu-id="6908e-113">您無法登入 Microsoft 365、Azure 或 Intune</span><span class="sxs-lookup"><span data-stu-id="6908e-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="6908e-114">在 Windows 10 上更新 Office 2016 build 16.0.7967 之後，登入後的連線問題</span><span class="sxs-lookup"><span data-stu-id="6908e-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="6908e-115">"很抱歉，您組織中的另一個帳戶已在這部電腦上登錄" （Office）</span><span class="sxs-lookup"><span data-stu-id="6908e-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="6908e-116">使用 ADFS 時疑難排解 Office 新式驗證的登入問題</span><span class="sxs-lookup"><span data-stu-id="6908e-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)