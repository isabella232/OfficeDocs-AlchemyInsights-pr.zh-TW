---
title: 交換傳統根網站與新式網站
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "2579"
- "9000687"
ms.openlocfilehash: dad7d7a52222dc09aea532714a93ca89c0d9ae19
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/07/2019
ms.locfileid: "36245933"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>交換傳統根網站與新式網站

如果您的環境設定成 [年 4 月 2019年之前，您可以變更至新式網站的根網站使用 Microsoft PowerShell:

- 如果您有不同的網站，您想要作為根網站時，您可以將 （分頁） 的根網站取代它。 
    - 使用[Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)封存原始網站時切換網站與其他網站的位置。 適用於小組網站 （未連線至群組） 及通訊網站。 

- 額外的功能將會引進推出，可讓您保留網站上，使用內容，但是在通訊網站轉換現有的網站。 
>[!Important]
>這些功能會逐步導入。 繼續進行若要檢查 Office 365 訊息中心的更新。 

## <a name="known-issues-with-swapping-sites"></a>交換網站的已知的問題

- 目標網站可能會傳回 「 找不到 」 (HTTP 404) 錯誤的短時間內。
- 內容必須重新編目要更新的搜尋索引。 沒有任何所需的手動步驟-這會自動完成。
- 取決於 「 靜態 」 連結 （例如檔案同步處理和 OneNote 檔案） 的任何項目將會需要手動修正。
- 如果來源網站組織新聞網站，更新 URL。取得所有組織新聞網站的清單。
- Project Server 網站可能需要驗證，以確保其仍然關聯正確。





