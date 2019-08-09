---
title: 新式網站作為根網站
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 260048db6c439183da8e0bb0c2dfa3c7475fca79
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/09/2019
ms.locfileid: "36269367"
---
# <a name="modern-site-as-root-site"></a>新式網站作為根網站

我們已開始導入可讓您將交換與新式網站您傳統網站的根網站的新功能。 使用[Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps)封存原始網站時切換網站與其他網站的位置。 適用於小組網站 （未連線至群組） 及通訊網站。 

>[!Important]
> 請勿刪除傳統的根網站以建立新式通訊網站。 Microsoft 不支援此。 刪除根網站會使所有的 SharePoint 網站組織中所有使用者，無法存取直到您還原的網站，或在相同的 URL 建立新的網站。 我們將通訊透過訊息中心這項功能。 您應該會開啟在您的租用戶中短時間內的功能。

## <a name="known-issues-with-swapping-sites"></a>交換網站的已知的問題
- 目標網站可能會傳回 「 找不到 」 (HTTP 404) 錯誤的短時間內。
- 內容必須重新編目要更新的搜尋索引。 並沒有手動步驟是這裡所需，這將會自動完成。
- 取決於 「 靜態 」 連結 （例如檔案同步處理和 OneNote 檔案） 的任何項目將會需要手動修正。
- Project Server 網站可能需要驗證，以確保其仍然關聯正確。 
