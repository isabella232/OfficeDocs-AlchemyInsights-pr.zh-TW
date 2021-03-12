---
title: 套用高級搜尋查詢的最佳作法
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736018"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>套用高級搜尋查詢的最佳作法

若要更快地取得結果，並避免執行複雜查詢時超時，請套用下列最佳作法：

- 嘗試新的查詢時，一定要使用限制，以避免取得極大的結果集。 此外，您也 `count` 可以使用來進行初始評估結果集的大小。
- 首先使用時間篩選。 理想狀況下，將您的查詢限制為七天。
- 在查詢的開頭，在時間篩選器之後，新增預期的篩選，以移除大部分的資料。
- 尋找完整的標記時，請使用 `has` 運算子而非 `contains` 。
- 針對特定欄執行搜尋，而不是在所有欄上執行搜尋。
- 當加入資料表時，請先以較少的列指定資料表。
- `project` 只從您已加入之資料表的必要欄。

若要深入瞭解，請參閱 [高級搜尋查詢最佳作法](https://go.microsoft.com/fwlink/?linkid=2144812)。
