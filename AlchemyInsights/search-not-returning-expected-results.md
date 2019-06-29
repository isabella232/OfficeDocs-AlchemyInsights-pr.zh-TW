---
title: 1491-搜尋-未傳回-預期結果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d25c1ef2e0e746432472a436cb11d25b5db5596c
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355868"
---
# <a name="content-search-not-returning-expected-results"></a>內容搜尋未傳回預期的結果

從 Office 365 安全性 & 規範中心執行內容搜尋時, 您可能會收到未預期的搜尋結果。 請考慮下列可能會影響搜尋結果的專案:

- **內容位置和搜尋條件**: 請確定您已選取適當的內容位置和搜尋條件。 如果您執行大型搜尋 (有許多位置), 請考慮將它分割成多個搜尋。

- **部分編制索引的專案**: 信箱中的[部分已編制索引的專案](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)會包含在預估的搜尋結果中。 不過, 在 SharePoint 和 OneDrive 中的網站已部分編制索引的專案不會包含在搜尋預估中。

- **搜尋失敗**: 搜尋大量信箱 (超過100000個信箱) 時, 您可能會收到搜尋錯誤, 如 CS008-009 和 CS012-002 等錯誤代碼。 在這種情況下, 請僅針對失敗的內容位置重試搜尋。 如需詳細資訊, 請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)。
