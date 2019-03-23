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
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776073"
---
# <a name="content-search-not-returning-expected-results"></a>未預期的結果傳回的內容搜尋

從 Office 365 安全性 & 合規性中心執行內容搜尋，您可能會收到未預期的搜尋結果。 請考慮下列事項，可能會影響您的搜尋結果：

- **內容的位置和搜尋條件**： 請確定您已選取適當的內容位置和搜尋條件。 如果您執行大型搜尋 （使用許多位置），請考慮將它分割成多個搜尋。

- **已局部編製索引的項目**： 預估的搜尋結果中隨附的信箱的[已局部編製索引的項目](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)。 不過，SharePoint 和 OneDrive 中的網站中的已局部編製索引項目不包含在搜尋估計值。

- **搜尋失敗**： 當您搜尋大量信箱 （超過 100000 信箱），您可能會收到搜尋錯誤，例如 CS008 009 和 CS012-002 錯誤碼)。 在此情況下，再試一次僅針對失敗的內容位置的搜尋。 請參閱[這篇文章](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)如需詳細資訊。
