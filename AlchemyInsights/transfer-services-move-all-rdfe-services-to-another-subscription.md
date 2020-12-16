---
title: 傳輸服務-將所有 RDFE 服務移至另一個訂閱
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "49681460"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="78294-102">傳輸服務-將所有 RDFE 服務移至另一個訂閱</span><span class="sxs-lookup"><span data-stu-id="78294-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="78294-103">**移動資源**</span><span class="sxs-lookup"><span data-stu-id="78294-103">**Move resources**</span></span>

<span data-ttu-id="78294-104">Azure 資源可使用 Azure 入口網站、Azure PowerShell、Azure CLI 或 REST API 移至相同訂閱下的其他 Azure 訂閱或資源群組，以移動資源。</span><span class="sxs-lookup"><span data-stu-id="78294-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="78294-105">您可以移動資源之前，請參閱：</span><span class="sxs-lookup"><span data-stu-id="78294-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="78294-106">移動資源前的檢查清單</span><span class="sxs-lookup"><span data-stu-id="78294-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="78294-107">可以移動的服務</span><span class="sxs-lookup"><span data-stu-id="78294-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="78294-108">如何驗證移動</span><span class="sxs-lookup"><span data-stu-id="78294-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="78294-109">服務的移動指導方針</span><span class="sxs-lookup"><span data-stu-id="78294-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="78294-110">若要將現有資源移至另一個資源群組或訂閱，您可以使用：</span><span class="sxs-lookup"><span data-stu-id="78294-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="78294-111">Azure 入口網站</span><span class="sxs-lookup"><span data-stu-id="78294-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="78294-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="78294-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="78294-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="78294-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="78294-114">REST API</span><span class="sxs-lookup"><span data-stu-id="78294-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="78294-115">教程： [將 Azure 資源移至另一個資源群組或訂閱](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="78294-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="78294-116">**疑難排解 Azure 資源管理員的錯誤**</span><span class="sxs-lookup"><span data-stu-id="78294-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="78294-117">請參閱下列文章，以瞭解一些常見的 Azure 部署錯誤，並收到資訊以加以解決。</span><span class="sxs-lookup"><span data-stu-id="78294-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="78294-118">如果您找不到您的部署錯誤的錯誤碼，請參閱 [find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code)。</span><span class="sxs-lookup"><span data-stu-id="78294-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="78294-119">疑難排解部署錯誤</span><span class="sxs-lookup"><span data-stu-id="78294-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="78294-120">疑難排解將 Azure 資源移至新的資源群組或訂閱</span><span class="sxs-lookup"><span data-stu-id="78294-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="78294-121">請注意，如果您想要升級您的 Azure 訂閱，例如從空閒切換成隨移即付即用，您必須轉換您的訂閱。</span><span class="sxs-lookup"><span data-stu-id="78294-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="78294-122">若要升級免費試用版，請參閱將 [您的免費試用版或 Microsoft 想像 Azure 訂閱升級為隨需付費](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription)。</span><span class="sxs-lookup"><span data-stu-id="78294-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="78294-123">若要變更隨用付費帳戶，請參閱將您的 [Azure 隨付即用訂閱變更為不同的服務](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer)。</span><span class="sxs-lookup"><span data-stu-id="78294-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="78294-124">**若要將 Azure 訂閱新增或關聯至您的 Azure Active Directory 租使用者：**</span><span class="sxs-lookup"><span data-stu-id="78294-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="78294-125">從 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade)中的 [訂閱] 頁面登入並選取您要使用的訂閱。</span><span class="sxs-lookup"><span data-stu-id="78294-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="78294-126">選取 [ **變更目錄**]。</span><span class="sxs-lookup"><span data-stu-id="78294-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="78294-127">查看顯示的任何警告，然後選取 [ **變更**]。</span><span class="sxs-lookup"><span data-stu-id="78294-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="78294-128">訂閱已變更目錄，您會收到一則成功的訊息。</span><span class="sxs-lookup"><span data-stu-id="78294-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="78294-129">使用 *目錄* 切換器移至新目錄。</span><span class="sxs-lookup"><span data-stu-id="78294-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="78294-130">最多可能需要10分鐘的時間，才能正確顯示所有專案。</span><span class="sxs-lookup"><span data-stu-id="78294-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="78294-131">**建譯的文件**</span><span class="sxs-lookup"><span data-stu-id="78294-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="78294-132">轉移 Azure 訂閱的擁有權</span><span class="sxs-lookup"><span data-stu-id="78294-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="78294-133">將資源移至新的資源群組或訂閱</span><span class="sxs-lookup"><span data-stu-id="78294-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="78294-134">使用 Azure 入口網站管理資源</span><span class="sxs-lookup"><span data-stu-id="78294-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
