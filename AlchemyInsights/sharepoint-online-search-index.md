---
title: 在 SharePoint Online 中管理搜尋字典
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 5319c2f1edc3e61074301f039736d2aa96bda47b
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758757"
---
# <a name="search-in-sharepoint-online"></a>在 SharePoint Online 中搜尋

內容必須經過編目並新增至搜尋索引, 使用者才能在 SharePoint Online 中找到他們搜尋的內容。 會根據預先定義的編目排程自動編目內容 (無法變更編目排程)。 編目程式會挑選自上次編目後已變更的內容, 並更新索引。 若要確保編目內容並更新索引, 請遵循下列步驟。

請確定可搜尋網站內容以找到內容。 如需詳細資訊, 請參閱[啟用網站上的內容以](https://docs.microsoft.com/sharepoint/make-site-content-searchable)供搜尋。

當您變更 managed 屬性, 或變更編目和 managed 屬性的對應時, 必須重新編目網站, 然後才會在搜尋索引中反映您的變更。 

因為您的變更是在搜尋架構中進行, 而不是實際執行的網站, 所以編目程式不會自動重新編制網站索引。 

如需詳細資訊, 請參閱[手動要求編目和重新索引網站、文件庫或清單](https://docs.microsoft.com/sharepoint/crawl-site-conten)。

 請至少等候24小時後, 手動要求編目和完整重新編制索引, 以查看您是否仍在遇到問題。 

如果在您啟動編目和完整重新編制索引後超過24小時, 請記錄支援案例。 在許多情況下, 我們已經在處理解決方案。 請至少為我們提供24小時的時間, 才可完成解決方案。

**重要**事項: 如果網站、檔 (文件庫) 或清單已刪除, 但仍顯示在搜尋結果中, 當嘗試存取時, 使用者應該會收到錯誤404檔案。 此問題應該記錄為支援案例, 以進一步進行調查。 



