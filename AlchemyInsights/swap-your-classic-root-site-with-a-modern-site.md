---
title: 將傳統的根網站與現代網站交換
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: f4831c6a232a4dee0f8f5ac0c83e4307221cfe2d
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741535"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>將傳統的根網站與現代網站交換

如果您的環境是在2019年4月之前設定，您可以使用 Microsoft PowerShell: 將您的根網站變更為現代網站。

- 如果您有不同的網站，您想要用來作為根網站，您可以將[根網站取代（換用）](https://docs.microsoft.com/sharepoint/modern-root-site) 。 
    - 使用[SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)在封存原始網站時，將網站的位置交換為另一個網站。 可用於兩個小組網站（未連接至群組）和通訊網站。 

- 將會很快引進其他功能，讓您繼續使用網站上的內容，但將現有網站轉換為通訊網站。 
>[!Important]
>這些功能將會逐步向之外進行匯總。 繼續檢查訊息中心是否有更新。 

## <a name="known-issues-with-swapping-sites"></a>交換網站的已知問題

- 目標網站可能會傳回一小段時間的「找不到」（HTTP 404）錯誤。
- 內容將需要重新編目更新搜尋索引。 不需要手動步驟，這將會自動完成。
- 任何依存于「靜態」連結的專案（例如，檔案同步處理及 OneNote 檔案）都必須手動修正。
- 如果來源網站為組織新聞網站，請更新 URL。取得所有組織新聞網站的清單。
- 可能需要驗證 Project Server 網站，以確保它們仍然有正確相關聯。
