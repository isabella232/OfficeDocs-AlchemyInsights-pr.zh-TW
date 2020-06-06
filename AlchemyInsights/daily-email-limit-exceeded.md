---
title: 超過每日電子郵件限制。 工作流程已暫停。
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580324"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="33141-103">超過每日電子郵件限制。</span><span class="sxs-lookup"><span data-stu-id="33141-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="33141-104">工作流程已暫停。</span><span class="sxs-lookup"><span data-stu-id="33141-104">Workflow is suspended.</span></span>

<span data-ttu-id="33141-105">在下列案例中，您可能會收到此錯誤：</span><span class="sxs-lookup"><span data-stu-id="33141-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="33141-106">您在使用 SharePoint 2010 或 SharePoint 2013 工作流程平臺類型的 SharePoint Online 中有工作流程。</span><span class="sxs-lookup"><span data-stu-id="33141-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="33141-107">工作流程設定為一次傳送自訂的電子郵件訊息給超過200位使用者、每天超過10000個收件者，或每分鐘超過30封郵件。</span><span class="sxs-lookup"><span data-stu-id="33141-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="33141-108">當您執行工作流程時，未傳送電子郵件訊息，您會注意到下列行為：</span><span class="sxs-lookup"><span data-stu-id="33141-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="33141-109">針對使用 SharePoint 2013 平臺類型的工作流程，請流覽至 [**工作流程狀態**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="33141-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="33141-110">在 [工作流程狀態] 頁面上，**內部狀態**會設定為 [**已啟動**]，而 [資訊] 氣球會顯示**無法傳送給收件**者。</span><span class="sxs-lookup"><span data-stu-id="33141-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="33141-111">若要解決此問題，請設定工作流程以傳送電子郵件，但不超過[Exchange Online 寄件者限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)。</span><span class="sxs-lookup"><span data-stu-id="33141-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="33141-112">例如，在工作流程中使用 pause，將電子郵件傳送至 Microsoft 365 群組、通訊群組或啟用郵件功能的安全性群組，或一次傳送郵件給超過200個收件者。</span><span class="sxs-lookup"><span data-stu-id="33141-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="33141-113">如需詳細資訊，請參閱下列[文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。</span><span class="sxs-lookup"><span data-stu-id="33141-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="33141-114">相關主題</span><span class="sxs-lookup"><span data-stu-id="33141-114">Related topics</span></span>
- [<span data-ttu-id="33141-115">建立流程</span><span class="sxs-lookup"><span data-stu-id="33141-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="33141-116">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="33141-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 