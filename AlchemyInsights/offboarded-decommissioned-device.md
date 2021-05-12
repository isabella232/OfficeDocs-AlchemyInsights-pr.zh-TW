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
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319170"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>從裝置庫存移除 offboarded 或解除授權裝置時的問題

Microsoft Defender for Endpoint 目前不允許從裝置庫存手動移除 offboarded 或解除授權裝置的裝置記錄。

基於安全性的考慮，裝置會在入口網站中維持為歷史記錄，最多180天。 不過，裝置資料會根據您設定的保留期間來清除。

**附注：** Offboarded 或解除授權的裝置會在七天后自動切換到 **非** 使用中狀態。 此外，過去30天內非使用中的裝置不會考慮反映組織威脅的資料，也不會影響裝置的漏洞管理洩密分數或 Microsoft 安全分數。
 
如果您仍不想要在裝置庫存模式中查看特定裝置，請嘗試放置裝置標籤，以從裝置庫存模式中篩選出解除授權的裝置。

如需詳細資訊，請參閱：

[Microsoft Defender for Endpoint service 中的下架裝置](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[威脅和弱點管理中的披露分數](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[修正 Microsoft Defender for Endpoint 中的狀況不良感應器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[如何有效地使用標記 (第1部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[如何有效地使用標記 (第2部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[如何有效地使用標記 (第3部分) ](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




