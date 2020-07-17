---
title: 與 filename 最佳
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750961"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="63f9e-102">「需要 Alchemy 標頭 H1，H2's 不會運作」。</span><span class="sxs-lookup"><span data-stu-id="63f9e-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="63f9e-103">用於 Alchemy 製作的最佳做法和指導方針：</span><span class="sxs-lookup"><span data-stu-id="63f9e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="63f9e-104">**不在資料夾中嵌套 Alchemy 洞察力**-這會中斷 url 結構。</span><span class="sxs-lookup"><span data-stu-id="63f9e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="63f9e-105">我們正在尋找修正這種情況。</span><span class="sxs-lookup"><span data-stu-id="63f9e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="63f9e-106">**AlchemyInsights**資料夾中的檔案應該會有小寫的檔案名，且空格（ex）為連字號。</span><span class="sxs-lookup"><span data-stu-id="63f9e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="63f9e-107">***使用方法-保留***。</span><span class="sxs-lookup"><span data-stu-id="63f9e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="63f9e-108">在自自訂欄位的[Alchemy 夥伴入口網站](https://alchemyportal.azurewebsites.net)中包含規則識別碼或 bucket 識別碼。</span><span class="sxs-lookup"><span data-stu-id="63f9e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="63f9e-109">前。</span><span class="sxs-lookup"><span data-stu-id="63f9e-109">ex.</span></span> <span data-ttu-id="63f9e-110">***ms. custom：100021***</span><span class="sxs-lookup"><span data-stu-id="63f9e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="63f9e-111">使用此檔案頂端的中繼資料做為範本。</span><span class="sxs-lookup"><span data-stu-id="63f9e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="63f9e-112">在「Alchemy 協力廠商」[入口網站](https://alchemyportal.azurewebsites.net)中，向下流覽至 [**客戶洞察力] 標題區段：** 並將其當作您的 H1 標題的起點，以供深入瞭解。</span><span class="sxs-lookup"><span data-stu-id="63f9e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="63f9e-113">Alchemy 真知灼見的上方必須只有一個 H1，否則會在生產中中斷。</span><span class="sxs-lookup"><span data-stu-id="63f9e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="63f9e-114">H2s 不會呈現任何一種，使用**粗體**或其他慣例表示個別的區段。</span><span class="sxs-lookup"><span data-stu-id="63f9e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="63f9e-115">接下來，在 [Alchemy 規則] 頁面的 [客戶洞察力] 區段中，使用草稿材料填滿本文。</span><span class="sxs-lookup"><span data-stu-id="63f9e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="63f9e-116">項目符號清單很正常</span><span class="sxs-lookup"><span data-stu-id="63f9e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="63f9e-117">編號清單太</span><span class="sxs-lookup"><span data-stu-id="63f9e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="63f9e-118">**粗體**及*斜體*為-ok</span><span class="sxs-lookup"><span data-stu-id="63f9e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="63f9e-119">連結應該會是「 **web**上的連結」/external 或**深層連結的 UI 元素**（而非內部連結）。</span><span class="sxs-lookup"><span data-stu-id="63f9e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="63f9e-120">目前並未正式支援圖片，但其位於藍圖。</span><span class="sxs-lookup"><span data-stu-id="63f9e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="63f9e-121">這實際上已經有點過長。</span><span class="sxs-lookup"><span data-stu-id="63f9e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="63f9e-122">最佳作法是大約400個字元---------------------------------</span><span class="sxs-lookup"><span data-stu-id="63f9e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="63f9e-123">準備好內容之後，請將其拉入即時分支。</span><span class="sxs-lookup"><span data-stu-id="63f9e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="63f9e-124">然後，移至「 [Alchemy 夥伴入口網站](https://alchemyportal.azurewebsites.net)」，並在 [url] 欄位中輸入該檔案名。</span><span class="sxs-lookup"><span data-stu-id="63f9e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 