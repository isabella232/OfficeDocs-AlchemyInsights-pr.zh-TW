---
title: 內容不會出現在 SharePoint 搜尋結果中
ms.author: tlarsen
author: tklarsen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: ca03c31def64e43935d734a17735b10373e5ca85b5f4ea0f0e886b9ea39884cd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54081601"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a>內容不會出現在 SharePoint 搜尋結果中

當預期的內容未出現在搜尋結果中時，請遵循下列疑難排解步驟：
  
1. 檢查包含預期內容的 **網站** 是否設定為允許內容出現在搜尋結果中。 依照在 [搜尋結果中顯示網站內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results)中的步驟進行。

2. 檢查包含預期內容的 **清單** 或文檔 **庫** ，是否設定為允許內容出現在搜尋結果中。 依照在 [搜尋結果中顯示清單或文件庫](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results)中的內容中的步驟進行。

3. 請確認頁面、檔或自訂的版面配置已發佈為 **主要版本。** 請遵循搜尋中的步驟3，[不會傳回 SharePoint Online 中的所有結果](https://go.microsoft.com/fwlink/?linkid=874525)。

4. 確認使用者具備查看內容的 **許可權** 。 遵循[SharePoint 中瞭解許可權等級](https://docs.microsoft.com/sharepoint/understanding-permission-levels)的步驟。
    
5. 如果已使用新增的 managed 屬性變更了搜尋架構、編輯 managed 屬性，或是移除 managed 屬性，則會需要要求編目及重新建立索引。 遵循 [手動要求編目及重新編制網站、文件庫或清單的索引](https://docs.microsoft.com/sharepoint/crawl-site-content)中的步驟，以 **重新編制內容索引**。 這可能需要一些時間，請等候24小時後檢查結果。

如需詳細資訊，請參閱 [讓網站上的內容](https://docs.microsoft.com/sharepoint/make-site-content-searchable)可供搜尋。 
  
