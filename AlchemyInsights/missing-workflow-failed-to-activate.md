---
title: 若要啟動遺失的工作流程失敗
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29917559"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="4dd05-102">若要啟動遺失的工作流程失敗</span><span class="sxs-lookup"><span data-stu-id="4dd05-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="4dd05-103">在 Microsoft SharePoint 網站集合，您無法新增至清單或文件庫的全域可重複使用的工作流程 （例如 「 核准-SharePoint 2010） 」。</span><span class="sxs-lookup"><span data-stu-id="4dd05-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="4dd05-104">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="4dd05-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="4dd05-105">SharePoint Designer 2013 中開啟之網站集合的根網站。</span><span class="sxs-lookup"><span data-stu-id="4dd05-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="4dd05-106">**網站物件**] 下選取 [**工作流程**。</span><span class="sxs-lookup"><span data-stu-id="4dd05-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="4dd05-107">**工作流程**功能區的 [**新增**] 區段中選取 [**可重複使用工作流程**]。</span><span class="sxs-lookup"><span data-stu-id="4dd05-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="4dd05-p101">在**建立可重複使用工作流程**表單中，輸入名稱 \* \* *Repair2010* \* \*。作為 [**平台類型**] 中，按一下 [ **SharePoint 2010 工作流程**，並再按一下 [**確定]**。</span><span class="sxs-lookup"><span data-stu-id="4dd05-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="4dd05-110">在 [**儲存\*\*\*\*工作流程**功能區] 區段中選取 [**發行**。</span><span class="sxs-lookup"><span data-stu-id="4dd05-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="4dd05-p102">**工作流程**功能區的 [**管理**] 區段中選取 [**全域發佈**]。在出現的 [確認] 對話方塊中選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="4dd05-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="4dd05-p103">在網頁瀏覽器中找出根網站的網站集合]，然後存取 [**網站設定** \> **網站集合功能**。然後，切換的**工作流程**功能：</span><span class="sxs-lookup"><span data-stu-id="4dd05-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="4dd05-115">·如果*啟動*此功能，按一下 [**停用，** 並再按一下 [**啟動**]。</span><span class="sxs-lookup"><span data-stu-id="4dd05-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="4dd05-116">·如果*已停用*此功能，按一下 [**啟動**]。</span><span class="sxs-lookup"><span data-stu-id="4dd05-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="4dd05-117">如需詳細資訊請參閱下列[文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="4dd05-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

