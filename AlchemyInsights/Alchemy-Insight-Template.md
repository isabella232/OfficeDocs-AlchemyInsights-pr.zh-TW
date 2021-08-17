---
title: 與 filename 最佳
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312816"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>「需要 Alchemy 標頭 H1，H2's 不會運作」。
用於 Alchemy 製作的最佳做法和指導方針：

1. **不在資料夾中嵌套 Alchemy Insights**，這會中斷 url 結構。 我們正在尋找修正這種情況。
1. **AlchemyInsights** 資料夾中的檔案應該會有小寫的檔案名，且空格（ex）為連字號。 **_使用方法-保留_**。
    1. 在自自訂欄位的 [Alchemy 夥伴入口網站](https://alchemyportal.azurewebsites.net) 中包含規則識別碼或 bucket 識別碼。 前。 ***ms. custom：100021***
1. 使用此檔案頂端的中繼資料做為範本。
1. 在「Alchemy 協力廠商」 [入口網站](https://alchemyportal.azurewebsites.net)中，向下流覽至 [ **客戶洞察力] 標題區段：** 並將其當作您的 H1 標題的起點，以供深入瞭解。 

**附注**： Alchemy Insights 最上層只有一個 H1，否則它們會在生產中中斷。 H2s 不會呈現任何一種，使用 **粗體** 或其他慣例表示個別的區段。
1. 接下來，使用 [Alchemy 規則] 頁面的 [Customer Insights] 區段中的拔模材料填滿本文。
    1. 項目符號清單很正常
    1. 編號清單太
    1. **粗體** 及 *斜體* 為-ok
    1. 連結應該會是「 **web** 上的連結」/external 或 **深層連結的 UI 元素**（而非內部連結）。
    1. 目前並未正式支援圖片，但其位於藍圖。

這實際上已經有點過長。 最佳作法是大約400個字元---------------------------------

準備好內容之後，請將其拉入即時分支。 然後，移至「 [Alchemy 夥伴入口網站](https://alchemyportal.azurewebsites.net) 」，並在 [url] 欄位中輸入該檔案名。 