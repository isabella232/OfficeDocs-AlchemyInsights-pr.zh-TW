---
title: 啟用成本管理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/08/2020
ms.locfileid: "49599062"
---
# <a name="enable-cost-management"></a><span data-ttu-id="2c699-102">啟用成本管理</span><span class="sxs-lookup"><span data-stu-id="2c699-102">Enable cost management</span></span>

<span data-ttu-id="2c699-103">**為您的組織停用成本是多少？**</span><span class="sxs-lookup"><span data-stu-id="2c699-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="2c699-104">使用 Enterprise 合約 (EA) 或 Microsoft Customer 合約 (MCA) 帳戶的組織，可停用成本資訊和價格資訊的存取權。</span><span class="sxs-lookup"><span data-stu-id="2c699-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="2c699-105">登入 Azure 入口網站後，使用者可以使用計費 APIs，以程式設計方式取得發票 (一選擇的) 和使用狀況詳細資料。</span><span class="sxs-lookup"><span data-stu-id="2c699-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="2c699-106">**如何允許其他使用者存取發票**</span><span class="sxs-lookup"><span data-stu-id="2c699-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="2c699-107">移至 Azure 入口網站中的 **訂閱 blade** 。</span><span class="sxs-lookup"><span data-stu-id="2c699-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="2c699-108">選取 [ **發票** ]，然後再 **存取 [發票**]。</span><span class="sxs-lookup"><span data-stu-id="2c699-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="2c699-109">開啟存取，然後儲存變更，以允許訂閱範圍的角色中的使用者下載發票。</span><span class="sxs-lookup"><span data-stu-id="2c699-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="2c699-110">帳戶管理員也可以設定透過電子郵件傳送發票。</span><span class="sxs-lookup"><span data-stu-id="2c699-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="2c699-111">若要深入瞭解，請參閱 [在電子郵件中取得您的發票](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?)。</span><span class="sxs-lookup"><span data-stu-id="2c699-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="2c699-112">**如何將使用者新增至計費讀取器角色**</span><span class="sxs-lookup"><span data-stu-id="2c699-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="2c699-113">移至 Azure 入口網站中的 **訂閱 blade** 。</span><span class="sxs-lookup"><span data-stu-id="2c699-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="2c699-114">選取 [ **(IAM]) 的 [存取控制** ]，然後按一下 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="2c699-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="2c699-115">選擇 [**選取角色**] 頁面中的 [**帳單讀取器**]。</span><span class="sxs-lookup"><span data-stu-id="2c699-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="2c699-116">輸入您要邀請之使用者的電子郵件，然後按一下 **[確定]** 以傳送邀請。</span><span class="sxs-lookup"><span data-stu-id="2c699-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="2c699-117">依照邀請電子郵件中提供的指示登入，以計費讀取者身分登入。</span><span class="sxs-lookup"><span data-stu-id="2c699-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="2c699-118">如需詳細資訊，請參閱 [授與帳單存取權](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in)。</span><span class="sxs-lookup"><span data-stu-id="2c699-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="2c699-119">**建議的檔**</span><span class="sxs-lookup"><span data-stu-id="2c699-119">**Recommended documents**</span></span>

- [<span data-ttu-id="2c699-120">透過 EA 入口網站啟用 DA 和 AO 視圖</span><span class="sxs-lookup"><span data-stu-id="2c699-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="2c699-121">成本管理中包含的成本</span><span class="sxs-lookup"><span data-stu-id="2c699-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="2c699-122">支援的 Microsoft Azure 提供</span><span class="sxs-lookup"><span data-stu-id="2c699-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="2c699-123">在成本分析中檢查成本</span><span class="sxs-lookup"><span data-stu-id="2c699-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="2c699-124">提供帳單資訊的存取權</span><span class="sxs-lookup"><span data-stu-id="2c699-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="2c699-125">檢查 Microsoft 客戶合約的存取權</span><span class="sxs-lookup"><span data-stu-id="2c699-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






