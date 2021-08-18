---
title: 從裝置庫存移除 offboarded 或解除授權裝置時的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 13865acb75b60a824c1dde9427c11471e980ea9e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324435"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>從裝置庫存移除 offboarded 或解除授權裝置時的問題

Microsoft Defender for Endpoint 目前不允許從裝置庫存手動移除 offboarded 或解除授權裝置的裝置記錄。

基於安全性的考慮，裝置會在入口網站中維持為歷史記錄，最多180天。 不過，裝置資料會根據您設定的保留期間來清除。

**附注：** Offboarded 或解除授權的裝置會在七天后自動切換到 **非** 使用中狀態。 此外，在過去30天內未使用的裝置，不會考慮反映組織威脅與弱點管理暴露程度或 Microsoft 安全評分為裝置的資料。
 
如果您仍不想要在裝置庫存模式中查看特定裝置，請嘗試放置裝置標籤，以從裝置庫存模式中篩選出解除授權的裝置。

如需詳細資訊，請參閱：

[Microsoft Defender for Endpoint service 中的下架裝置](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/offboard-machines.md)

[威脅與弱點管理中的披露分數](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[修正 Microsoft Defender for Endpoint 中的狀況不良感應器](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[如何有效地使用標記 (第1部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[如何有效地使用標記 (第2部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[如何有效地使用標記 (第3部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




