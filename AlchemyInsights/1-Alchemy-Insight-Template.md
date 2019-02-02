---
title: '相同檔名為最佳 [規則 #-說明]'
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 278a26f4b986a85e33442baef690d3bb44462ace
ms.sourcegitcommit: 32355b76d45b730a069575efeec708149d4aeaa3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/01/2019
ms.locfileid: "29697121"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="da5ec-102">需要的魔力標頭 H1、 H2 的未運作。</span><span class="sxs-lookup"><span data-stu-id="da5ec-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="da5ec-103">最佳作法和魔力製作的指導方針：</span><span class="sxs-lookup"><span data-stu-id="da5ec-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="da5ec-p101">**未巢狀處理資料夾中的魔力前瞻**-這會自動換行的 url 結構。我們要尋找到修正這。</span><span class="sxs-lookup"><span data-stu-id="da5ec-p101">**Do not nest Alchemy Insights in folders**- this will break the url structure. We're looking into fixing this.</span></span>
1. <span data-ttu-id="da5ec-106">在 [檔案名稱應有規則 ID 和[魔力協力廠商入口網站](https://alchemyportal.azurewebsites.net)中的規則名稱**AlchemyInsights**資料夾中的檔案。</span><span class="sxs-lookup"><span data-stu-id="da5ec-106">Files in the **AlchemyInsights** folder should have Rule ID and Rule Name from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the filename.</span></span>
    1. <span data-ttu-id="da5ec-p102">例如***976-How-to-enable-litigation-hold***</span><span class="sxs-lookup"><span data-stu-id="da5ec-p102">ex. ***976-How-to-enable-litigation-hold***</span></span>
1. <span data-ttu-id="da5ec-p103">使用此檔案頂端的中繼資料為您的範本。還不是必要的。</span><span class="sxs-lookup"><span data-stu-id="da5ec-p103">Use the metadata at the top of this file as your template. Nothing else is required.</span></span>
1. <span data-ttu-id="da5ec-111">在[魔力協力廠商入口網站](https://alchemyportal.azurewebsites.net)中，瀏覽至 [] 區段**客戶洞察力標題：** 與據您 H1 標題使用，以開始點。</span><span class="sxs-lookup"><span data-stu-id="da5ec-111">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="da5ec-p104">魔力前瞻必須僅限單一 H1 頂端或他們會在生產環境中會自動換行。H2s 不轉譯如此使用**粗體**或其他慣例分送給帶有表示不同的章節。</span><span class="sxs-lookup"><span data-stu-id="da5ec-p104">Alchemy Insights MUST have only a single H1 at the top or they will break in production. H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="da5ec-114">接下來，填滿使用草稿材料魔力規則] 頁面的 [客戶前瞻] 區段中的內文文字</span><span class="sxs-lookup"><span data-stu-id="da5ec-114">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="da5ec-115">是正常的項目符號清單</span><span class="sxs-lookup"><span data-stu-id="da5ec-115">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="da5ec-116">太編號清單</span><span class="sxs-lookup"><span data-stu-id="da5ec-116">Numbered lists too</span></span>
    1. <span data-ttu-id="da5ec-117">**粗體**和*斜體*是 a-ok</span><span class="sxs-lookup"><span data-stu-id="da5ec-117">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="da5ec-118">連結應該永遠為其中一個 **[連結至 web] / 外部**OR **UI 元素的深層連結**、 不內部的連結。</span><span class="sxs-lookup"><span data-stu-id="da5ec-118">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>

<span data-ttu-id="da5ec-p105">與這是真正已經有點太長。最佳做法是即將 400 個字元為--</span><span class="sxs-lookup"><span data-stu-id="da5ec-p105">And this is really already a bit too long. Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="da5ec-p106">一旦您的內容已準備好，則會提取至 live 分支。然後，移至[魔力協力廠商入口網站](https://alchemyportal.azurewebsites.net)並在 [url] 欄位中輸入檔案名稱。請務必檢閱及發佈的獨到"yes"表示，然後按一下 [更新規則。**（這會更加美觀入口網站-釋放推出新版本中。）**
 ![url] 欄位](media/for-content-team.PNG)</span><span class="sxs-lookup"><span data-stu-id="da5ec-p106">Once your content is ready, pull it to the live branch. Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field. Make sure Insight reviewed and published says "yes" and then click Update Rule. **(This will look prettier in the new version of the portal - releasing soon.)**
![url field](media/for-content-team.PNG)</span></span>

