---
title: 將傳統的根網站與現代網站交換
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 7209595f5cda9b31e53241d9d5696fa584ff5e5ab3d237aae28542bf7aec9398
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940810"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>將傳統的根網站與現代網站交換

如果您的環境是在2019年4月之前設定，您可以使用 Microsoft PowerShell: 將您的根網站變更為現代網站。

- 如果您有不同的網站，您想要用來作為根網站，您可以將 [ 根網站的 (換) ](https://docs.microsoft.com/sharepoint/modern-root-site) 取代。 
    - 使用 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 在封存原始網站時，將網站的位置交換為另一個網站。 可用於兩個小組網站 (未連接至群組) 和通訊網站。 

- 將會很快引進其他功能，讓您繼續使用網站上的內容，但將現有網站轉換為通訊網站。 
>[!Important]
>這些功能將會逐步向之外進行匯總。 繼續檢查訊息中心是否有更新。 

## <a name="known-issues-with-swapping-sites"></a>交換網站的已知問題

- 目標網站可能會在 HTTP 404) 錯誤的一小段時間內傳回「找不到」 (。
- 內容將需要重新編目更新搜尋索引。 不需要手動步驟，這將會自動完成。
- 任何依存于「靜態」連結 (（例如檔案同步處理及 OneNote 檔案）的內容，) 將需要手動修正。
- 如果來源網站為組織新聞網站，請更新 URL。 取得所有組織新聞網站的清單。
- Project您可能需要驗證服務器網站，以確保它們仍然有正確關聯。
