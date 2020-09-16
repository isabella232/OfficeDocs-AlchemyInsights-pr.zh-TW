---
title: 未傳送工作流程電子郵件
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748980"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a><span data-ttu-id="e9564-102">未傳送 SharePoint 清單或文件庫的工作流程電子郵件</span><span class="sxs-lookup"><span data-stu-id="e9564-102">Workflow email is not being sent for a SharePoint list or library</span></span>

1. <span data-ttu-id="e9564-103">來自工作流程的電子郵件不會傳送給所有使用者或只傳送給特定使用者，否則您會看到錯誤 **電子郵件無法傳送。請確定電子郵件具有有效的收件**者。</span><span class="sxs-lookup"><span data-stu-id="e9564-103">Email from workflows are not sent to all users or only specific users, or you see the error **The e-mail message cannot be sent. Make sure the e-mail has a valid recipient**.</span></span>

    <span data-ttu-id="e9564-104">檢查使用者是否存在於該網站集合的 [ **所有人員** ] 許可權群組中 (使用者資訊清單) 。</span><span class="sxs-lookup"><span data-stu-id="e9564-104">Check if the user exist in the **All People** permissions group (user information list) for that site collection.</span></span>  <span data-ttu-id="e9564-105">URL: <tenant> sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx 的範例 direct？MembershipGroupId = 0</span><span class="sxs-lookup"><span data-stu-id="e9564-105">Sample direct URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx?MembershipGroupId=0</span></span>

    - <span data-ttu-id="e9564-106">如果使用者不存在，請確定使用者已登入頁面。</span><span class="sxs-lookup"><span data-stu-id="e9564-106">If the user does not exist, make sure the user is signed into the page.</span></span> 
    - <span data-ttu-id="e9564-107">如果是外部使用者，請確定已接受其邀請。</span><span class="sxs-lookup"><span data-stu-id="e9564-107">If it is an external user, make sure that their invitation has been accepted.</span></span>
    - <span data-ttu-id="e9564-108">如果使用者確實存在於許可權群組中，請確定電子郵件地址正確無誤。</span><span class="sxs-lookup"><span data-stu-id="e9564-108">If the user does exist in the permissions group, make sure the email address is correct.</span></span>
    - <span data-ttu-id="e9564-109">若未在這裡設定使用者的電子郵件地址，則會為該使用者建立範例警示，以強制將該使用者帳戶從 SharePoint 的使用者設定檔同步處理至此網站集合。</span><span class="sxs-lookup"><span data-stu-id="e9564-109">If the users email address is not set here, then create a sample alert for that user which forces the sync of that user account from User Profiles of SharePoint to this site collection.</span></span>
 
2. <span data-ttu-id="e9564-110">來自工作流程的電子郵件會傳送給網站集合管理員，但不會傳送給其他使用者，也不會查看錯誤 **HTTP 禁止訪問 <span>HTTPs：</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**。</span><span class="sxs-lookup"><span data-stu-id="e9564-110">Email from workflows are sent to the site collection administrators but not to other users and see the error **HTTP Forbidden to <span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**.</span></span>
 

    <span data-ttu-id="e9564-111">[當您傳送電子郵件給 SharePoint 群組時，](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)請參閱「拒絕存取」。</span><span class="sxs-lookup"><span data-stu-id="e9564-111">See [Access Denied when you send an email to a SharePoint group](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups).</span></span>

    <span data-ttu-id="e9564-112">此外，請確認「 **限制存取使用者許可權鎖定模式** 」網站集合功能未作用中。</span><span class="sxs-lookup"><span data-stu-id="e9564-112">Also, verify that the **Limited-access user permission lockdown mode** site collection feature is not active.</span></span>


## <a name="related-topics"></a><span data-ttu-id="e9564-113">相關主題</span><span class="sxs-lookup"><span data-stu-id="e9564-113">Related topics</span></span>
<span data-ttu-id="e9564-114">想要在 SharePoint Online 中試用 Microsoft 流程嗎？</span><span class="sxs-lookup"><span data-stu-id="e9564-114">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="e9564-115">建立流程</span><span class="sxs-lookup"><span data-stu-id="e9564-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="e9564-116">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="e9564-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


