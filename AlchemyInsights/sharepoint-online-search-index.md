---
title: 搜尋 SharePoint Online
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: 3c3f6384172b2b4d59db6059618572db11059228
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36507622"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a>內容編目和編製索引 SharePoint Online 中

內容必須被編目並新增至使用者尋找項目他們透過其中搜尋的 SharePoint Online 中的搜尋索引。 內容會自動編目根據預先定義的編目排程 （不能變更編目排程）。 編目程式挑選自前次編目以來已變更及更新的索引的內容。 若要確保編目內容，以及更新索引，請注意下列事項：

- 請確定可以找到內容[製作網站內容可供搜尋](https://docs.microsoft.com/sharepoint/make-site-content-searchable)。

- 當您已變更的 managed 的屬性，或您已變更的對應的編目及 managed 屬性，該網站必須在重新編目，才能變更會反映在搜尋索引中。 

    搜尋結構描述中，而非實際網站進行變更，因為編目程式將不會自動重新編製索引之網站。 

    如需詳細資訊，請參閱[手動要求編目和重新編製索引的網站、 文件庫或清單](https://docs.microsoft.com/sharepoint/crawl-site-conten)。

- 請至少等候 24 小時之後以手動方式要求編目和完整重新編製索引以查看是否仍有問題。 

    如果您起始的編目和完整重新編製索引以來超過 24 小時，請登支援案例。 在許多情況下，我們已使用的方案。 請讓我們至少 24 小時才能完成解決方案。

> [!IMPORTANT]
> 如果網站、 文件 （檔案庫） 或清單已遭刪除，仍會顯示在搜尋結果中，使用者應該會收到**錯誤 404 找不到檔案**時，嘗試對其進行存取。 這個問題應該記錄為進一步調查的支援案例。 



