---
title: 為什麼會停用 [新增預算] 按鈕？
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
- "9003547"
- "6464"
ms.openlocfilehash: 426a54ea22490dcc47f40fd990654b2cf051a058
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822626"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a><span data-ttu-id="27df2-102">為什麼會停用 [新增預算] 按鈕？</span><span class="sxs-lookup"><span data-stu-id="27df2-102">Why is the Add budget button disabled for me?</span></span>

<span data-ttu-id="27df2-103">若要建立預算，您需要下列其中一個許可權：</span><span class="sxs-lookup"><span data-stu-id="27df2-103">To create a budget, you need one of the following permissions:</span></span>

- <span data-ttu-id="27df2-104">管理群組、訂閱、資源群組範圍</span><span class="sxs-lookup"><span data-stu-id="27df2-104">Management Group, Subscription, Resource Group Scopes</span></span>
- <span data-ttu-id="27df2-105">成本管理參與者</span><span class="sxs-lookup"><span data-stu-id="27df2-105">Cost Management Contributor</span></span>
- <span data-ttu-id="27df2-106">擁有者</span><span class="sxs-lookup"><span data-stu-id="27df2-106">Owner</span></span>
- <span data-ttu-id="27df2-107">投稿者</span><span class="sxs-lookup"><span data-stu-id="27df2-107">Contributor</span></span>
- <span data-ttu-id="27df2-108">僅限企業客戶：登記、部門、帳戶範圍</span><span class="sxs-lookup"><span data-stu-id="27df2-108">Enterprise Customer Only: Enrollment, Department, Account Scopes</span></span>
- <span data-ttu-id="27df2-109">註冊管理員 (在登記範圍設定預算) </span><span class="sxs-lookup"><span data-stu-id="27df2-109">Enrollment Admin (set budget at Enrollment scope)</span></span>
- <span data-ttu-id="27df2-110">部門管理員 (在部門範圍內設定預算) </span><span class="sxs-lookup"><span data-stu-id="27df2-110">Department Admin (set budget at Department scope)</span></span>
- <span data-ttu-id="27df2-111">帳戶擁有人 (設定預算 at 帳戶範圍) </span><span class="sxs-lookup"><span data-stu-id="27df2-111">Account Owner (set budget at Account scope)</span></span>
- <span data-ttu-id="27df2-112">僅限現代客戶合約：帳單帳戶、帳單設定檔、發票區段範圍</span><span class="sxs-lookup"><span data-stu-id="27df2-112">Modern Customer Agreement Only: Billing Account, Billing Profile, Invoice Section Scopes</span></span>
- <span data-ttu-id="27df2-113">Azure 訂閱建立者</span><span class="sxs-lookup"><span data-stu-id="27df2-113">Azure subscription creator</span></span>

<span data-ttu-id="27df2-114">**當當月成本已過預算時，我已建立預算。為什麼我未收到警示？**</span><span class="sxs-lookup"><span data-stu-id="27df2-114">**I created a budget when my cost for the current month was already over-budget. Why did I not receive an alert?**</span></span>  
<span data-ttu-id="27df2-115">當您建立預算時，如果您已超過指定的成本閾值，將不會觸發警示。</span><span class="sxs-lookup"><span data-stu-id="27df2-115">If you have already exceeded a given cost threshold when you create a budget that alert will not fire.</span></span> <span data-ttu-id="27df2-116">新迴圈開始之後，如果您違反臨界值，就會觸發警示。</span><span class="sxs-lookup"><span data-stu-id="27df2-116">Once a new cycle begins, if you breach the threshold then the alert will fire.</span></span>

<span data-ttu-id="27df2-117">**當我超過其中一個定義的預算警示閾值時，應何時收到警示？**</span><span class="sxs-lookup"><span data-stu-id="27df2-117">**When should I expect to receive an alert after I exceed one of my defined budget alert thresholds?**</span></span>  
<span data-ttu-id="27df2-118">每4小時會評估預算。</span><span class="sxs-lookup"><span data-stu-id="27df2-118">Budgets are evaluated every 4 hours.</span></span> <span data-ttu-id="27df2-119">使用狀況資料到達預算系統至少需要8小時。</span><span class="sxs-lookup"><span data-stu-id="27df2-119">It takes a minimum of 8 hours for usage data to reach the budgets system.</span></span> <span data-ttu-id="27df2-120">在此情況下，當您超過臨界值後，可能需要12小時才會觸發警示。</span><span class="sxs-lookup"><span data-stu-id="27df2-120">Given this, alerts may take as long as 12 hours to fire after you exceed a threshold.</span></span>

<span data-ttu-id="27df2-121">**為什麼當我選取月或帳單月重設期間時，停用開始日期按鈕？**</span><span class="sxs-lookup"><span data-stu-id="27df2-121">**Why is the Start date button disabled when I select a Month or Billing month reset period?**</span></span>  
<span data-ttu-id="27df2-122">在選取計費月份的情況下，會將預算對應至目前的行事曆月份或目前的計費期間 () 。</span><span class="sxs-lookup"><span data-stu-id="27df2-122">Budgets are aligned to the current calendar month or current billing period (in the case where Billing Month is selected).</span></span> <span data-ttu-id="27df2-123">因此，我們為您預先填入此值。</span><span class="sxs-lookup"><span data-stu-id="27df2-123">Therefore, we pre-populate this value for you.</span></span>

<span data-ttu-id="27df2-124">**為何在預算創造經驗中看不到成本的圖形？**</span><span class="sxs-lookup"><span data-stu-id="27df2-124">**Why do I not see a graph of my costs in the budget creation experience?**</span></span>  
<span data-ttu-id="27df2-125">我們至少需要2個月的成本資料，才能呈現圖形以協助您建立預算。</span><span class="sxs-lookup"><span data-stu-id="27df2-125">We need a minimum of 2 months of cost data before we can render a graph to assist you with budget creation.</span></span>

<span data-ttu-id="27df2-126">**為什麼我無法針對剛才建立的訂閱設定預算？**</span><span class="sxs-lookup"><span data-stu-id="27df2-126">**Why can't I set a budget against a subscription I just created?**</span></span>  
<span data-ttu-id="27df2-127">在建立訂閱後，在為數據設定預算之前，會花24-48 小時的時間進行處理。</span><span class="sxs-lookup"><span data-stu-id="27df2-127">After the creation of a subscription, the data takes 24-48 hours to process before setting a budget against it.</span></span>

<span data-ttu-id="27df2-128">**預算 API 資源**</span><span class="sxs-lookup"><span data-stu-id="27df2-128">**Budget API Resources**</span></span>

- <span data-ttu-id="27df2-129">[預算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用來建立和更新預算的作業。</span><span class="sxs-lookup"><span data-stu-id="27df2-129">[Budgets API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to create and update budgets.</span></span> <span data-ttu-id="27df2-130">使用預算 API，您可以設定預算臨界值，並設定在您接近該臨界值時，要激發的多個警示。</span><span class="sxs-lookup"><span data-stu-id="27df2-130">Using the Budgets API, you can set a budget threshold and configure multiple alerts to fire as you approach that threshold.</span></span> <span data-ttu-id="27df2-131">警示可觸發電子郵件或 Azure 動作群組，以執行自動化。</span><span class="sxs-lookup"><span data-stu-id="27df2-131">Alerts can trigger an email or an Azure Action Group to perform automation.</span></span> <span data-ttu-id="27df2-132">附注：此 API 的篩選不會與查詢 API 篩選/維度對齊。</span><span class="sxs-lookup"><span data-stu-id="27df2-132">Note: Filtering for this API does not align with Query API filtering / dimensions.</span></span>
- <span data-ttu-id="27df2-133">[預算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)：使用超過 v1 的成本篩選功能建立預算。</span><span class="sxs-lookup"><span data-stu-id="27df2-133">[Budgets API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json): Create budgets with greater cost filtering capabilities than v1.</span></span> <span data-ttu-id="27df2-134">篩選會對應至查詢和維度 APIs 中所用的合約。</span><span class="sxs-lookup"><span data-stu-id="27df2-134">Filtering aligns to the contract used in our Query and Dimensions APIs.</span></span> <span data-ttu-id="27df2-135">這是建議的預算 API，以用於向前移動。</span><span class="sxs-lookup"><span data-stu-id="27df2-135">This is the recommended budgets API to use moving forward.</span></span>
- <span data-ttu-id="27df2-136">[維度](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供作業，以在各種範圍下取得您使用狀況的支援維度。</span><span class="sxs-lookup"><span data-stu-id="27df2-136">[Dimensions](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get supported dimensions for your usage under a variety of scopes.</span></span> <span data-ttu-id="27df2-137">使用維度 API，您可以取得維度的清單，這些維度可做為使用查詢 API 產生查詢的輸入。</span><span class="sxs-lookup"><span data-stu-id="27df2-137">Using the Dimensions API, you can retrieve a list of dimensions that can be used as inputs for generating queries with the Query API.</span></span>
- <span data-ttu-id="27df2-138">[查詢](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供作業，以根據您提供的查詢取得匯總成本和使用方式資料。</span><span class="sxs-lookup"><span data-stu-id="27df2-138">[Query](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support): Provides operations to get aggregated cost and usage data based on the query you supply.</span></span> <span data-ttu-id="27df2-139">使用查詢 API，您可以指定您想要的篩選、排序及群組，以供從維度 API) 存取的所有可用維度 (。</span><span class="sxs-lookup"><span data-stu-id="27df2-139">Using the Query API, you can specify your desired filtering, sorting and grouping on all available dimensions (which are accessed from the Dimensions API).</span></span>

<span data-ttu-id="27df2-140">**預測成本**</span><span class="sxs-lookup"><span data-stu-id="27df2-140">**Forecasted Costs**</span></span>

<span data-ttu-id="27df2-141">**為何在成本分析中看不到成本的預測？**</span><span class="sxs-lookup"><span data-stu-id="27df2-141">**Why don’t I see forecasts for my costs in Cost Analysis?**</span></span>  
<span data-ttu-id="27df2-142">預測預測可能在成本分析中遺失的原因有多種，有些如下：</span><span class="sxs-lookup"><span data-stu-id="27df2-142">There are multiple reasons why the forecast projection might be missing for you in Cost Analysis, some of them are as follows:</span></span>

1. <span data-ttu-id="27df2-143">如果成本資料超過10天，將不會載入預測圖表。</span><span class="sxs-lookup"><span data-stu-id="27df2-143">If your cost data is less than 10 days old, the forecast chart will not load.</span></span> <span data-ttu-id="27df2-144">模型至少需要10天的最近成本資料，以進行準確的預測</span><span class="sxs-lookup"><span data-stu-id="27df2-144">The model requires at least 10 days of recent cost data for accurate projections</span></span>
2. <span data-ttu-id="27df2-145">如果您已選取 [已歷史日期]，則預測圖表將不會顯示。</span><span class="sxs-lookup"><span data-stu-id="27df2-145">If you have selected historic dates, then the forecast chart will not be visible.</span></span> <span data-ttu-id="27df2-146">請選取要顯示的預測圖表的日期範圍及未來日期</span><span class="sxs-lookup"><span data-stu-id="27df2-146">Please select a date range with future dates for the forecast chart to be displayed</span></span>
3. <span data-ttu-id="27df2-147">如果您的帳戶有多種貨幣，預測圖表只會為「USD 中的所有成本」專案成本。</span><span class="sxs-lookup"><span data-stu-id="27df2-147">If your account has multiple currencies, the forecast chart will only project costs for 'All costs in USD'</span></span>

<span data-ttu-id="27df2-148">**為何變更我的資源時，預測不會變更？**</span><span class="sxs-lookup"><span data-stu-id="27df2-148">**Why doesn’t the forecast change when I make changes to my resources?**</span></span>  
<span data-ttu-id="27df2-149">預測模型需要數天的時間來考慮帳戶的變更，而且不會根據資源變更進行立即預測</span><span class="sxs-lookup"><span data-stu-id="27df2-149">The forecast model requires a couple of days to account for changes in the account and does not make immediate projections based on change in resources</span></span>  
<span data-ttu-id="27df2-150">在資源增加或減少的較大步驟中，模型會花很長的時間調整至這些變更，以應對異常</span><span class="sxs-lookup"><span data-stu-id="27df2-150">For larger steps of increase or decrease in resources, the model will take slightly longer to adjust to these changes to account for anomalies</span></span>

<span data-ttu-id="27df2-151">**為什麼我的預測會在我進行保留或 Marketplace 購買之後增加？**</span><span class="sxs-lookup"><span data-stu-id="27df2-151">**Why does my forecast increase after I make a reservation or Marketplace purchase?**</span></span>  
<span data-ttu-id="27df2-152">預測模型會考慮「實際成本」，而不會個別考慮使用和購買。如果是一次性購買，模型會在10天后減少預測，以考慮突然增加成本。</span><span class="sxs-lookup"><span data-stu-id="27df2-152">The forecast model considers your 'Actual Cost' and does not account for usage and purchase separately.For a one-time purchase, the model will decrease the projections after 10 days to account for the sudden increase in costs</span></span>

<span data-ttu-id="27df2-153">**我想要查看單一維度的預測 (例如。儀錶)**</span><span class="sxs-lookup"><span data-stu-id="27df2-153">**I want to see forecasts for a single dimension (eg. Meter)**</span></span>  
<span data-ttu-id="27df2-154">預測目前支援總成本預測，而不是個別計量。</span><span class="sxs-lookup"><span data-stu-id="27df2-154">Forecast currently supports total cost projections and not for individual meters.</span></span> <span data-ttu-id="27df2-155">因此，當「分組依據」維度時，預測將會成為維度中所有專案的總計</span><span class="sxs-lookup"><span data-stu-id="27df2-155">Hence, when 'Grouped by' a dimension, the projections will be for total of all items in the dimension</span></span>

<span data-ttu-id="27df2-156">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="27df2-156">**Recommended Documents**</span></span>

- [<span data-ttu-id="27df2-157">何謂 Azure 成本管理？</span><span class="sxs-lookup"><span data-stu-id="27df2-157">What is Azure Cost Management?</span></span>](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="27df2-158">Azure 成本管理的最佳作法</span><span class="sxs-lookup"><span data-stu-id="27df2-158">Azure Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="27df2-159">分析成本和開支</span><span class="sxs-lookup"><span data-stu-id="27df2-159">Analyze your costs and spending</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="27df2-160">探索和分析成本與成本分析</span><span class="sxs-lookup"><span data-stu-id="27df2-160">Explore and analyze costs with Cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="27df2-161">Azure 成本管理：價格</span><span class="sxs-lookup"><span data-stu-id="27df2-161">Azure Cost Management: Pricing</span></span>](https://azure.microsoft.com/services/cost-management/#pricing)
- [<span data-ttu-id="27df2-162">在成本分析中檢查成本</span><span class="sxs-lookup"><span data-stu-id="27df2-162">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [<span data-ttu-id="27df2-163">影片教學課程：在 Azure 入口網站中建立預算</span><span class="sxs-lookup"><span data-stu-id="27df2-163">Video tutorial: Create a budget in the Azure portal</span></span>](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [<span data-ttu-id="27df2-164">查看和自訂預算的必要條件</span><span class="sxs-lookup"><span data-stu-id="27df2-164">Prerequisites for viewing and customizing budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [<span data-ttu-id="27df2-165">建立及管理預算</span><span class="sxs-lookup"><span data-stu-id="27df2-165">Create and manage budgets</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [<span data-ttu-id="27df2-166">使用 Azure 動作群組和預算 API 設定自動化</span><span class="sxs-lookup"><span data-stu-id="27df2-166">Configure automation with Azure Action Groups and Budgets API</span></span>](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [<span data-ttu-id="27df2-167">使用成本警示來監控使用方式和開支</span><span class="sxs-lookup"><span data-stu-id="27df2-167">Use cost alerts to monitor usage and spending</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="27df2-168">成本管理的最佳作法</span><span class="sxs-lookup"><span data-stu-id="27df2-168">Cost Management best practices</span></span>](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

<span data-ttu-id="27df2-169">**教學課程影片**</span><span class="sxs-lookup"><span data-stu-id="27df2-169">**Tutorial videos**</span></span>

- [<span data-ttu-id="27df2-170">在 Azure 入口網站中建立預算</span><span class="sxs-lookup"><span data-stu-id="27df2-170">Create a budget in the Azure portal</span></span>](https://go.microsoft.com/fwlink/?linkid=2146761)
- [<span data-ttu-id="27df2-171">使用預算 API 和動作群組管理成本</span><span class="sxs-lookup"><span data-stu-id="27df2-171">Manage costs with the Budgets API and Action Groups</span></span>](https://go.microsoft.com/fwlink/?linkid=2147038)