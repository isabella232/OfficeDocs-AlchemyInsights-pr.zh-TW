---
title: 1491-search-not-returning-expected-results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964815"
---
# <a name="content-search-not-returning-expected-results"></a>內容搜尋未傳回預期的結果

從 Office 365 安全性 & 規範中心執行內容的搜尋，您可能會收到非預期的搜尋結果。請考慮下列事項可能會影響搜尋結果：

- **內容的位置與搜尋條件**： 請確定已選取適當的內容位置並搜尋條件。如果您已執行大型搜尋 （以及更多的位置），請考慮分割成多個搜尋。

- **部分編製索引的項目**： 從信箱[部分編製索引的項目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)包含在預估的搜尋結果中。不過，部分已編製索引的項目從 SharePoint 和 OneDrive 中的網站不包含在搜尋評估。

- **搜尋失敗**： 搜尋信箱 （超過 100000 信箱） 的數目、 時可能會取得搜尋錯誤，例如 CS008 009 和 CS012 002 錯誤碼)。在此例中再試一次僅針對失敗的內容位置搜尋。請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)如需詳細資訊。
