---
title: 1491-搜尋-未傳回-預期結果
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: d0707af19b0299f7257a10a20ab38f47860308fb
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43709218"
---
# <a name="content-search-not-returning-expected-results"></a>內容搜尋未傳回預期的結果

從 Microsoft 365 security & 合規性中心執行內容搜尋時，您可能會收到意外的搜尋結果。 請考慮可能影響搜尋結果的下列專案：

- **內容位置和搜尋條件**：請確定您已選取適當的內容位置和搜尋條件。 如果您執行大型搜尋（有許多位置），請考慮將其分割為多個搜尋。

- **部分索引項目目**：信箱中的[部分已編制索引的專案](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search)會包含在預估的搜尋結果中。 不過，搜尋評估中不會包含從 SharePoint 和 OneDrive 中的網站部分編制索引的專案。

- **搜尋失敗**：搜尋大量信箱（超過100000個信箱）時，您可能會收到搜尋錯誤，例如 CS008-009 和 CS012-002 等錯誤代碼。 在此情況下，只會針對失敗的內容位置，重試搜尋。 如需詳細資訊，請參閱[本文](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search)。
