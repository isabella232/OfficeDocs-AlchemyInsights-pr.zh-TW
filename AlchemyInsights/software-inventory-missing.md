---
title: 軟體庫存遺失或不正確
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/26/2021
ms.locfileid: "52658047"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a>軟體庫存遺失或不正確

威脅與弱點管理 (TVM) 中的軟體清查是貴組織中具有官方通用平台列舉 (CPE) 的已知軟體清單。

沒有官方 CPE 的軟體產品不會發佈弱點。 清查也包含詳細資料，例如廠商名稱、弱點數目、威脅，以及暴露的裝置數目。

裝置上的軟體變更通常會在兩小時內反映在安全性入口網站中。 不過，有時可能需要較長的時間。 目前無法強制同步處理；此為持續進行的評估。

如果您進行軟體變更，但 5 小時後變更未正確反映在 TVM 中，請遵循下列步驟：

1. 檢查軟體證據區段，以了解偵測軟體的方式。
1. 確定軟體受到支援。 軟體只能在裝置層級顯示，即使威脅與弱點管理目前不支援該軟體也一樣。 不過，只可使用有限的資料。
1. 如需從入口網站報告錯誤的步驟，請參閱[報告錯誤](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy)。
   
    **注意**：從 MDE 入口網站報告錯誤是進行工程設計的單向通道。 如果問題緊急，請開立支援票證。

如需詳細資訊，請參閱[軟體清查 - 威脅與弱點管理](/microsoft-365/security/defender-endpoint/tvm-software-inventory)。