---
title: 修正傳輸規則
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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034745"
---
# <a name="fix-transport-rules"></a>修正傳輸規則

自訂郵件流程規則會影響此郵件。 若要查看確切的規則，請執行下列動作：

1. 在提交結果的 [ **其他資訊**] 下，記下 **GUID** 或 **原則名稱**。
2. 啟動 Exchange 管理命令介面。 如需詳細資訊，請參閱[Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432)。
3. 使用提交) 中的 GUID 執行此命令 (：  **Get-TransportRule 身分 "GUID" | fl * 描述***
4. 請複查描述，以查看影響郵件的設定條件。

若要深入瞭解，請參閱 [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)。
