---
title: 根據 Ediscovery 匯出的 Chromium 瀏覽器使用 Microsoft Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3473"
- "3100022"
ms.openlocfilehash: a583896b5aa8e73be5e932a729c380acc8092e73b2151647c999f9a7b69669b6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998378"
---
# <a name="using-microsoft-edge-based-on-chromium-browsers-for-ediscovery-export"></a>根據 Ediscovery 匯出的 Chromium 瀏覽器使用 Microsoft Edge

由於最近的變更，因此預設不會啟用 Microsoft Edge 瀏覽器的 ClickOnce 支援。 若要繼續使用 Microsoft 365 eDiscovery 匯出工具，您必須使用 Microsoft Internet Explorer 或啟用 Microsoft Edge 中的 ClickOnce 支援。 

若要根據 Chromium 在 Microsoft Edge 中啟用 ClickOnce 支援： 
1. 在您的 Microsoft Edge 瀏覽器中，請 edge://flags/#edge-按一下一次。
2. 對於 ClickOnce 支援選項，將值從 [**預設**] 或 [**已停用**] 變更為 [**已啟用**]。 
3. 在瀏覽器視窗底部，選取 [ **重新開機**]。 <br>
 變更將會在重新開機 Microsoft Edge 後生效。 

如需有關如何安裝匯出工具及步驟的詳細資訊，請參閱： [ 匯出內容搜尋結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。