---
title: 相同檔名，最好
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800036"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="fccc7-102">需要的魔力標頭 H1、 H2 的沒有作用。</span><span class="sxs-lookup"><span data-stu-id="fccc7-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="fccc7-103">最佳作法和魔力製作的指導方針：</span><span class="sxs-lookup"><span data-stu-id="fccc7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="fccc7-104">**進行巢狀處理資料夾中的魔力觀點**-這會自動換行的 url 結構。</span><span class="sxs-lookup"><span data-stu-id="fccc7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="fccc7-105">我們要尋找到修正這。</span><span class="sxs-lookup"><span data-stu-id="fccc7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="fccc7-106">**AlchemyInsights**資料夾中的檔案應該有以連字號 ex 空間小寫檔名。</span><span class="sxs-lookup"><span data-stu-id="fccc7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="fccc7-107">***how-以-啟用-訴訟暫止的狀態***。</span><span class="sxs-lookup"><span data-stu-id="fccc7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="fccc7-108">在 ms.custom] 欄位中包含[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)] 中的規則 ID 或 bucket 識別碼。</span><span class="sxs-lookup"><span data-stu-id="fccc7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="fccc7-109">ex。</span><span class="sxs-lookup"><span data-stu-id="fccc7-109">ex.</span></span> <span data-ttu-id="fccc7-110">***ms.custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="fccc7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="fccc7-111">使用此檔案頂端的中繼資料的其餘部分，為您的範本。</span><span class="sxs-lookup"><span data-stu-id="fccc7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="fccc7-112">在 「[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)中，瀏覽 [下一節**客戶深入了解標題：** 和深入了解您 H1 標題，做為起點指向用於。</span><span class="sxs-lookup"><span data-stu-id="fccc7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="fccc7-113">魔力觀點必須有只有單一 H1 頂端或他們將會中斷在生產環境中。</span><span class="sxs-lookup"><span data-stu-id="fccc7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="fccc7-114">H2s 未呈現如此使用**粗體**或其他慣例，以表示不同的章節。</span><span class="sxs-lookup"><span data-stu-id="fccc7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="fccc7-115">接下來，填寫使用草稿材料魔力規則] 頁面的 [客戶深入資訊] 區段中的內文文字</span><span class="sxs-lookup"><span data-stu-id="fccc7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="fccc7-116">是正常的項目符號清單</span><span class="sxs-lookup"><span data-stu-id="fccc7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="fccc7-117">太編號清單</span><span class="sxs-lookup"><span data-stu-id="fccc7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="fccc7-118">**粗體**和*斜體格式*是 a-ok</span><span class="sxs-lookup"><span data-stu-id="fccc7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="fccc7-119">連結應該永遠為其中一個 **」 網頁的連結 」 / 外部**OR **UI 元素的深層連結**、 不內部連結。</span><span class="sxs-lookup"><span data-stu-id="fccc7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="fccc7-120">圖片不受正式支援現階段，但它位於藍圖。</span><span class="sxs-lookup"><span data-stu-id="fccc7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="fccc7-121">這確實已經是有點太長。</span><span class="sxs-lookup"><span data-stu-id="fccc7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="fccc7-122">最佳作法是 400 個字元為--</span><span class="sxs-lookup"><span data-stu-id="fccc7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="fccc7-123">準備您的內容之後，請至 live 分支提取。</span><span class="sxs-lookup"><span data-stu-id="fccc7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="fccc7-124">然後，移至[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)，並在 [url] 欄位輸入檔案名稱。</span><span class="sxs-lookup"><span data-stu-id="fccc7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 