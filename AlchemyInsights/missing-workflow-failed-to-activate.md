---
title: 無法啟動遺失的工作流程
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667077"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="caab0-102">無法啟動遺失的工作流程</span><span class="sxs-lookup"><span data-stu-id="caab0-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="caab0-103">在 Microsoft SharePoint 網站集合中，您無法新增全域可重複使用的工作流程 (例如「核准-SharePoint 2010」 ) 至清單或文件庫。</span><span class="sxs-lookup"><span data-stu-id="caab0-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="caab0-104">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="caab0-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="caab0-105">在 SharePoint 設計工具2013中開啟網站集合的根網站。</span><span class="sxs-lookup"><span data-stu-id="caab0-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="caab0-106">在 [ **網站物件**] 底下，選取 [ **工作流程**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="caab0-107">在 [**工作流程**] 功能區的**新**區段中，選取 [**可重複使用的工作流程**]</span><span class="sxs-lookup"><span data-stu-id="caab0-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="caab0-108">在 [ **建立可重複使用的工作流程** ] 表單上，輸入名稱 \* \* *Repair2010* \* \*。</span><span class="sxs-lookup"><span data-stu-id="caab0-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="caab0-109">針對 [ **平臺類型**]，按一下 [ **SharePoint 2010 工作流程**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="caab0-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="caab0-110">在 [**工作流程**] 功能區的 [**儲存**] 區段中，選取 [**發佈**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="caab0-111">在 [**工作流程**] 功能區的 [**管理**] 區段中，選取 [**全域發佈**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="caab0-112">在出現的確認對話方塊中，選取 **[確定**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="caab0-113">在網頁瀏覽器中，找出網站集合的根網站，然後存取 **網站設定** \> **網站集合的功能**。</span><span class="sxs-lookup"><span data-stu-id="caab0-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="caab0-114">然後，切換 **工作流程** 功能：</span><span class="sxs-lookup"><span data-stu-id="caab0-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="caab0-115">·如果已  *啟用*  該功能，請按一下 [ **停用]，** 然後按一下 [ **啟動**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="caab0-116">·如果  *停用*  此功能，請按一下 [ **啟動**]。</span><span class="sxs-lookup"><span data-stu-id="caab0-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="caab0-117">如需詳細資訊，請參閱下列 [文章](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="caab0-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

