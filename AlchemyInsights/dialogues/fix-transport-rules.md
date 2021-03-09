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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568491"
---
# <a name="fix-transport-rules"></a>修正傳輸規則

自訂郵件流程規則會影響此郵件。 若要查看確切的規則，請執行下列動作：

1. 在提交結果的 [ **其他資訊**] 下，記下 **GUID** 或 **原則名稱**。
2. 啟動 Exchange 管理命令介面。 如需詳細資訊，請參閱 [開啟 Exchange 管理命令](https://go.microsoft.com/fwlink/?linkid=2101432)介面。
3. 使用提交) 中的 GUID 執行此命令 (：  **Get-TransportRule 身分 "GUID" | fl * 描述***
4. 請複查描述，以查看影響郵件的設定條件。

若要深入瞭解，請參閱 [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)。
