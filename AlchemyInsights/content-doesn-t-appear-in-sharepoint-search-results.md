---
title: 內容不會出現在 SharePoint 搜尋結果中
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363789"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>內容不會出現在 SharePoint 搜尋結果中

如果預期的內容未出現在搜尋結果中, 請遵循下列疑難排解步驟:
  
1. 檢查包含預期內容的**網站**是否設定為允許內容出現在搜尋結果中。 請依照在[搜尋結果中顯示網站內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)的步驟進行。

2. 檢查包含預期內容的**清單**或文檔**庫**是否已設定為允許內容出現在搜尋結果中。 請依照 [在[搜尋結果中顯示清單](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的內容] 或 [文件庫] 中的步驟。

3. 確認頁面、檔或自訂頁面配置已發佈為**主要版本。** 請遵循搜尋中的步驟 3,[不會傳回 SharePoint Online 中的所有結果](https://go.microsoft.com/fwlink/?linkid=874525)。

4. 確認使用者具有查看內容的**許可權**。 請依照[瞭解 SharePoint 中的許可權層級](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels)中的步驟進行。
    
5. 如果已透過新增 managed 屬性來變更搜尋架構、編輯 managed 屬性, 或是移除 managed 屬性, 則需要進行編目和重新編制索引。 [請依照手動要求編目和重新編制網站、文件庫或清單的索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步驟,**重新編制內容索引**。 這可能需要一段時間, 請等候24小時後再檢查結果。

如需詳細資訊, 請參閱[啟用網站上的內容以](https://docs.microsoft.com/sharepoint/make-site-content-searchable)供搜尋。 
  
