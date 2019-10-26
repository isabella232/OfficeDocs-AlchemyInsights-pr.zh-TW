---
title: 無法啟動工作流程
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: 2d85dcf9111d48cb529c583c733823b404eb3188
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/25/2019
ms.locfileid: "36738080"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="7da96-102">無法啟動工作流程</span><span class="sxs-lookup"><span data-stu-id="7da96-102">Workflow is not starting</span></span>

- <span data-ttu-id="7da96-103">無法啟動 SharePoint 2010 和 SharePoint 2013 工作流程。</span><span class="sxs-lookup"><span data-stu-id="7da96-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="7da96-104">如果無法啟動您的工作流程，可能有的暫時的服務問題： 使用者可能會遇到間歇性延遲與工作流程進度。</span><span class="sxs-lookup"><span data-stu-id="7da96-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="7da96-105">檢查[服務健康狀況儀表板](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)若要查看您的組織會受到影響。</span><span class="sxs-lookup"><span data-stu-id="7da96-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="7da96-106">如果您第一次看到此問題以來超過 24 小時，請登支援票證。</span><span class="sxs-lookup"><span data-stu-id="7da96-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7da96-107">在許多情況下，我們已使用的方案。</span><span class="sxs-lookup"><span data-stu-id="7da96-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7da96-108">請讓我們至少 24 小時才能完成解決方案。</span><span class="sxs-lookup"><span data-stu-id="7da96-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="7da96-109">SharePoint 2010 工作流程延遲開始。</span><span class="sxs-lookup"><span data-stu-id="7da96-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="7da96-110">如果在大型的批次中觸發工作流程時，發生此情況。</span><span class="sxs-lookup"><span data-stu-id="7da96-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="7da96-111">（例如，當多個項目會新增一次）。</span><span class="sxs-lookup"><span data-stu-id="7da96-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="7da96-112">工作流程是並非特別設計用來執行即時，因此延遲是所設計的行為。</span><span class="sxs-lookup"><span data-stu-id="7da96-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="7da96-113">如果工作流程是複雜的 「 可延伸物件標記語言 」 (XMOL)，編譯可能會很慢。</span><span class="sxs-lookup"><span data-stu-id="7da96-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="7da96-114">請檢查[這](https://support.microsoft.com//kb/3043697)篇文章。</span><span class="sxs-lookup"><span data-stu-id="7da96-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="7da96-115">您應該簡化工作流程或重新設計使用 Microsoft SharePoint 2013 工作流程平台類型。</span><span class="sxs-lookup"><span data-stu-id="7da96-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="7da96-116">如果您的工作流程歷程記錄有變大，您可能想要清除的項目，或建立新的歷程記錄清單。</span><span class="sxs-lookup"><span data-stu-id="7da96-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="7da96-117">[清除工作流程歷程記錄](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)的詳細資訊：</span><span class="sxs-lookup"><span data-stu-id="7da96-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="7da96-118">相關主題</span><span class="sxs-lookup"><span data-stu-id="7da96-118">Related topics</span></span>
<span data-ttu-id="7da96-119">想要在 SharePoint Online 中的 Microsoft Flow？</span><span class="sxs-lookup"><span data-stu-id="7da96-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="7da96-120">建立流程</span><span class="sxs-lookup"><span data-stu-id="7da96-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="7da96-121">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="7da96-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


