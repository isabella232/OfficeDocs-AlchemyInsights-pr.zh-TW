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
ms.openlocfilehash: 1263662184948ed1e77e3abacd17babf4aa033ed1ecec29b4c4afc26d6da56f0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53954653"
---
# <a name="why-is-the-add-budget-button-disabled-for-me"></a>為什麼會停用 [新增預算] 按鈕？

若要建立預算，您需要下列其中一個許可權：

- 管理群組、訂閱、資源群組範圍
- 成本管理參與者
- 擁有者
- 投稿者
- Enterprise僅限客戶：登記、部門、帳戶範圍
- 註冊管理員 (在登記範圍設定預算) 
- 部門管理員 (在部門範圍內設定預算) 
- 帳戶擁有人 (設定預算 at 帳戶範圍) 
- 僅限現代客戶合約：帳單帳戶、帳單設定檔、發票區段範圍
- Azure 訂閱建立者

**當當月成本已過預算時，我已建立預算。為什麼我未收到警示？**  
當您建立預算時，如果您已超過指定的成本閾值，將不會觸發警示。 新迴圈開始之後，如果您違反臨界值，就會觸發警示。

**當我超過其中一個定義的預算警示閾值時，應何時收到警示？**  
每4小時會評估預算。 使用狀況資料到達預算系統至少需要8小時。 在此情況下，當您超過臨界值後，可能需要12小時才會觸發警示。

**為什麼當我選取月或帳單月重設期間時，停用開始日期按鈕？**  
在選取計費月份的情況下，會將預算對應至目前的行事曆月份或目前的計費期間 () 。 因此，我們為您預先填入此值。

**為何在預算創造經驗中看不到成本的圖形？**  
我們至少需要2個月的成本資料，才能呈現圖形以協助您建立預算。

**為什麼我無法針對剛才建立的訂閱設定預算？**  
在建立訂閱後，在為數據設定預算之前，會花24-48 小時的時間進行處理。

**預算 API 資源**

- [預算 API v1](https://docs.microsoft.com/rest/api/consumption/budgets?WT.mc_id=Portal-Microsoft_Azure_Support)：提供用來建立和更新預算的作業。 使用預算 API，您可以設定預算臨界值，並設定在您接近該臨界值時，要激發的多個警示。 警示可觸發電子郵件或 Azure 動作群組，以執行自動化。 附注：此 API 的篩選不會與查詢 API 篩選/維度對齊。
- [預算 API v2](https://github.com/Azure/azure-rest-api-specs/blob/master/specification/cost-management/resource-manager/Microsoft.CostManagement/preview/2019-04-01-preview/examples/CreateOrUpdateBudget.json)：使用超過 v1 的成本篩選功能建立預算。 篩選會對應至查詢和維度 APIs 中所用的合約。 這是建議的預算 API，以用於向前移動。
- [維度](https://docs.microsoft.com/rest/api/cost-management/dimensions?WT.mc_id=Portal-Microsoft_Azure_Support)：提供作業，以在各種範圍下取得您使用狀況的支援維度。 使用維度 API，您可以取得維度的清單，這些維度可做為使用查詢 API 產生查詢的輸入。
- [查詢](https://docs.microsoft.com/rest/api/cost-management/query?WT.mc_id=Portal-Microsoft_Azure_Support)：提供作業，以根據您提供的查詢取得匯總成本和使用方式資料。 使用查詢 API，您可以指定您想要的篩選、排序及群組，以供從維度 API) 存取的所有可用維度 (。

**預測成本**

**為何在成本分析中看不到成本的預測？**  
預測預測可能在成本分析中遺失的原因有多種，有些如下：

1. 如果成本資料超過10天，將不會載入預測圖表。 模型至少需要10天的最近成本資料，以進行準確的預測
2. 如果您已選取 [已歷史日期]，則預測圖表將不會顯示。 請選取要顯示的預測圖表的日期範圍及未來日期
3. 如果您的帳戶有多種貨幣，預測圖表只會為「USD 中的所有成本」專案成本。

**為何變更我的資源時，預測不會變更？**  
預測模型需要數天的時間來考慮帳戶的變更，而且不會根據資源變更進行立即預測  
在資源增加或減少的較大步驟中，模型會花很長的時間調整至這些變更，以應對異常

**為什麼我的預測會在我進行保留或 Marketplace 購買之後增加？**  
預測模型會考慮「實際成本」，而不會個別考慮使用和購買。如果是一次性購買，模型會在10天后減少預測，以考慮突然增加成本。

**我想要查看單一維度的預測 (例如。儀錶)**  
預測目前支援總成本預測，而不是個別計量。 因此，當「分組依據」維度時，預測將會成為維度中所有專案的總計

**建譯的文件**

- [何謂 Azure 成本管理？](https://docs.microsoft.com/azure/cost-management/overview-cost-mgt?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理的最佳作法](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)
- [分析成本和開支](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [探索和分析成本與成本分析](https://docs.microsoft.com/azure/cost-management/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Azure 成本管理：價格](https://azure.microsoft.com/services/cost-management/#pricing)
- [在成本分析中檢查成本](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support#review-costs-in-cost-analysis)
- [影片教學課程：在 Azure 入口網站中建立預算](https://www.youtube.com/watch?v=ExIVG_Gr45A&t=4s)
- [查看和自訂預算的必要條件](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#prerequisites)
- [建立及管理預算](https://docs.microsoft.com/azure/cost-management-billing/costs/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#create-a-budget-in-the-azure-portal)
- [使用 Azure 動作群組和預算 API 設定自動化](https://docs.microsoft.com/azure/cost-management/tutorial-acm-create-budgets?WT.mc_id=Portal-Microsoft_Azure_Support#trigger-an-action-group)
- [使用成本警示來監控使用方式和開支](https://docs.microsoft.com/azure/cost-management/cost-mgt-alerts-monitor-usage-spending?WT.mc_id=Portal-Microsoft_Azure_Support)
- [成本管理的最佳作法](https://docs.microsoft.com/azure/cost-management/cost-mgt-best-practices?WT.mc_id=Portal-Microsoft_Azure_Support)  

**教學課程影片**

- [在 Azure 入口網站中建立預算](https://go.microsoft.com/fwlink/?linkid=2146761)
- [使用預算 API 和動作群組管理成本](https://go.microsoft.com/fwlink/?linkid=2147038)