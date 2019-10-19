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
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>需要的魔力標頭 H1、 H2 的沒有作用。
最佳作法和魔力製作的指導方針：

1. **進行巢狀處理資料夾中的魔力觀點**-這會自動換行的 url 結構。 我們要尋找到修正這。
1. **AlchemyInsights**資料夾中的檔案應該有以連字號 ex 空間小寫檔名。 ***how-以-啟用-訴訟暫止的狀態***。
    1. 在 ms.custom] 欄位中包含[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)] 中的規則 ID 或 bucket 識別碼。 ex。 ***ms.custom: 100021***
1. 使用此檔案頂端的中繼資料的其餘部分，為您的範本。
1. 在 「[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)中，瀏覽 [下一節**客戶深入了解標題：** 和深入了解您 H1 標題，做為起點指向用於。 
    > [!NOTE]
    > 魔力觀點必須有只有單一 H1 頂端或他們將會中斷在生產環境中。 H2s 未呈現如此使用**粗體**或其他慣例，以表示不同的章節。
1. 接下來，填寫使用草稿材料魔力規則] 頁面的 [客戶深入資訊] 區段中的內文文字
    1. 是正常的項目符號清單
    1. 太編號清單
    1. **粗體**和*斜體格式*是 a-ok
    1. 連結應該永遠為其中一個 **」 網頁的連結 」 / 外部**OR **UI 元素的深層連結**、 不內部連結。
    1. 圖片不受正式支援現階段，但它位於藍圖。

這確實已經是有點太長。 最佳作法是 400 個字元為--

準備您的內容之後，請至 live 分支提取。 然後，移至[魔力合作夥伴入口網站](https://alchemyportal.azurewebsites.net)，並在 [url] 欄位輸入檔案名稱。 