---
title: 未開始工作流程
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
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403734"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="4c80b-102">未開始工作流程</span><span class="sxs-lookup"><span data-stu-id="4c80b-102">Workflow is not starting</span></span>

- <span data-ttu-id="4c80b-103">SharePoint 2010 和 SharePoint 2013 工作流程無法啟動。</span><span class="sxs-lookup"><span data-stu-id="4c80b-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="4c80b-104">如果您的工作流程未開始，可能是暫時性的服務問題，使用者可能會遇到工作流程進度的延遲延遲。</span><span class="sxs-lookup"><span data-stu-id="4c80b-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="4c80b-105">請檢查 [服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home/servicehealth) ，以查看您的組織是否受到影響。</span><span class="sxs-lookup"><span data-stu-id="4c80b-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="4c80b-106">如果從您第一次看到此問題起已經過去超過24小時，請記錄支援票證。</span><span class="sxs-lookup"><span data-stu-id="4c80b-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="4c80b-107">多數情況下，我們已經著手研究解決方案。</span><span class="sxs-lookup"><span data-stu-id="4c80b-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="4c80b-108">請至少為我們提供24小時的時間來完成解決方案。</span><span class="sxs-lookup"><span data-stu-id="4c80b-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="4c80b-109">SharePoint 2010 工作流程在開始時延遲。</span><span class="sxs-lookup"><span data-stu-id="4c80b-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="4c80b-110">如果工作流程以大量批次觸發，便會發生這種情況。</span><span class="sxs-lookup"><span data-stu-id="4c80b-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="4c80b-111"> (例如，一次新增多個專案) 。</span><span class="sxs-lookup"><span data-stu-id="4c80b-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="4c80b-112">工作流程並非設計為即時執行，所以延遲是設計行為。</span><span class="sxs-lookup"><span data-stu-id="4c80b-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="4c80b-113">如果工作流程是複雜且可擴展的物件標記語言 (XMOL) ，編譯可能會很慢。</span><span class="sxs-lookup"><span data-stu-id="4c80b-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="4c80b-114">請[參閱本文。](https://support.microsoft.com//kb/3043697)</span><span class="sxs-lookup"><span data-stu-id="4c80b-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="4c80b-115">您應該簡化工作流程，或使用 Microsoft SharePoint 2013 工作流程平臺類型進行重新設計。</span><span class="sxs-lookup"><span data-stu-id="4c80b-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="4c80b-116">如果您的工作流程歷程記錄已增加，您可能想要清除專案或建立新的歷程記錄清單。</span><span class="sxs-lookup"><span data-stu-id="4c80b-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="4c80b-117">詳細資訊： [清除工作流程歷程記錄](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="4c80b-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="4c80b-118">相關主題</span><span class="sxs-lookup"><span data-stu-id="4c80b-118">Related topics</span></span>
<span data-ttu-id="4c80b-119">想要在 SharePoint Online 中試用 Microsoft 流程嗎？</span><span class="sxs-lookup"><span data-stu-id="4c80b-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="4c80b-120">建立流程</span><span class="sxs-lookup"><span data-stu-id="4c80b-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="4c80b-121">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="4c80b-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
