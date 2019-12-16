---
title: 已超過每日的電子郵件限制。 暫止工作流程。
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
ms.openlocfilehash: 3cad5d8305da0a5db9a85888793350a062e6aed6
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053108"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="ee8a8-103">超過限制每日的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="ee8a8-104">暫止工作流程。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-104">Workflow is suspended.</span></span>

<span data-ttu-id="ee8a8-105">在下列案例中可能會收到此錯誤：</span><span class="sxs-lookup"><span data-stu-id="ee8a8-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="ee8a8-106">您可以讓工作流程在 SharePoint Online 中使用 SharePoint 2010 或 SharePoint 2013 工作流程平台類型。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="ee8a8-107">工作流程已設定為傳送自訂電子郵件訊息給 200 位以上的使用者在時間、 10000 個以上的收件者每日或每分鐘 30 個以上的郵件。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="ee8a8-108">當您執行的工作流程時，不會傳送電子郵件訊息，並請注意下列行為：</span><span class="sxs-lookup"><span data-stu-id="ee8a8-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="ee8a8-109">使用 [SharePoint 2013 平台類型為工作流程，您瀏覽至 [**工作流程狀態**] 頁面上。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="ee8a8-110">在 [工作流程狀態] 頁面**內部的狀態**設定為 [**已啟動**，並資訊註解方塊會顯示**無法傳送給收件者**。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="ee8a8-111">若要解決此問題，設定您的工作流程不超過[Exchange Online 寄件者限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)傳送電子郵件訊息。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="ee8a8-112">例如，使用工作流程中的暫停、 傳送電子郵件給 Office 365 群組、 通訊群組或擁有郵件功能的安全性群組，或將郵件傳送至 200 個收件者，一次。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="ee8a8-113">如需詳細資訊，請參閱下列[文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。</span><span class="sxs-lookup"><span data-stu-id="ee8a8-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="ee8a8-114">相關主題</span><span class="sxs-lookup"><span data-stu-id="ee8a8-114">Related topics</span></span>
- [<span data-ttu-id="ee8a8-115">建立流程</span><span class="sxs-lookup"><span data-stu-id="ee8a8-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ee8a8-116">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="ee8a8-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 