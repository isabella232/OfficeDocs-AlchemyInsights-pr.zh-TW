---
title: 工作流程電子郵件就不會被傳送
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 783bf0a5721aa5db7088432c71e06cac6dc90513
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059595"
---
# <a name="workflow-email-is-not-being-sent"></a><span data-ttu-id="50eae-102">工作流程電子郵件就不會被傳送</span><span class="sxs-lookup"><span data-stu-id="50eae-102">Workflow email is not being sent</span></span>

1. <span data-ttu-id="50eae-103">從工作流程的電子郵件並不會傳送給所有使用者或只有特定使用者，或您會看到錯誤**電子郵件無法傳送。請確定該電子郵件具有有效收件者**。</span><span class="sxs-lookup"><span data-stu-id="50eae-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

<span data-ttu-id="50eae-104">檢查使用者存在於該網站集合的**所有人員**的權限群組 （使用者資訊清單）。</span><span class="sxs-lookup"><span data-stu-id="50eae-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="50eae-105">範例直接 URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx 嗎？MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="50eae-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

- <span data-ttu-id="50eae-106">如果使用者不存在，請確定使用者登入] 頁面。</span><span class="sxs-lookup"><span data-stu-id="50eae-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
- <span data-ttu-id="50eae-107">如果是外部使用者，請確定已經接受其邀請。</span><span class="sxs-lookup"><span data-stu-id="50eae-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
- <span data-ttu-id="50eae-108">如果使用者的權限] 群組中存在，請務必電子郵件地址正確無誤。</span><span class="sxs-lookup"><span data-stu-id="50eae-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
- <span data-ttu-id="50eae-109">如果使用者電子郵件地址不在此設定，然後建立該使用者可從的 SharePoint 使用者設定檔會強制使用者帳戶同步處理至這個網站集合的範例警示。</span><span class="sxs-lookup"><span data-stu-id="50eae-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="50eae-110">從工作流程的電子郵件傳送給網站集合管理員，但未提供給其他使用者，並查看錯誤\*\*HTTP 禁止以<spam> <spam> \*\* <spam> <spam>。</span><span class="sxs-lookup"><span data-stu-id="50eae-110">Email from Workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <spam><spam>https://URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**<spam><spam>.</span></span>
 

<span data-ttu-id="50eae-111">請參閱[「 拒絕存取 」 時傳送電子郵件傳送到群組](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups)。</span><span class="sxs-lookup"><span data-stu-id="50eae-111">See [Access Denied when sent email to groups](https://docs.microsoft.com/sharepoint/support/server-admin/access-denied-when-send-an-email-to-groups).</span></span>

<span data-ttu-id="50eae-112">此外，確認**限制存取使用者的權限鎖定模式**網站集合功能為非作用中。</span><span class="sxs-lookup"><span data-stu-id="50eae-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>

## <a name="related-topics"></a><span data-ttu-id="50eae-113">相關主題</span><span class="sxs-lookup"><span data-stu-id="50eae-113">Related topics</span></span>
- [<span data-ttu-id="50eae-114">建立流程</span><span class="sxs-lookup"><span data-stu-id="50eae-114">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="50eae-115">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="50eae-115">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


