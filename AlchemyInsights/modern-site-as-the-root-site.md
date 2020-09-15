---
title: 新式網站作為根網站
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666861"
---
# <a name="modern-site-as-root-site"></a>新式網站為根網站

我們已開始推出新功能，可讓您將 [傳統網站根網站與現代網站交換](https://docs.microsoft.com/sharepoint/modern-root-site)。 使用 [SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) 在封存原始網站時，將網站的位置交換為另一個網站。 可用於兩個小組網站 (未連接至群組) 和通訊網站。

>[!Important]
> 請勿刪除傳統的根網站來建立新式的通訊網站。 Microsoft 不支援此功能。 刪除根網站會使所有的使用者都無法存取組織中的所有 SharePoint 網站，直到您還原網站或在相同 URL 上建立新網站為止。 我們將透過訊息中心來傳遞這項功能。 您應該會在您的租使用者中立即開啟此功能。

## <a name="known-issues-with-swapping-sites"></a>交換網站的已知問題
- 目標網站可能會在 HTTP 404) 錯誤的一小段時間內傳回「找不到」 (。
- 內容將需要重新編目更新搜尋索引。 沒有必要手動步驟，這將會自動完成。
- 任何依存于「靜態」連結 (（例如檔案同步處理及 OneNote 檔案）的內容，) 將需要手動修正。
- 可能需要驗證 Project Server 網站，以確保它們仍然有正確相關聯。 
