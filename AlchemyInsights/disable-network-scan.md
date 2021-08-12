---
title: 停用網路掃描
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/25/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001464"
- "3492"
ms.openlocfilehash: 7e67a45b6f4d4b18f47ce55a0fde20f826498c5d25c4a6dec4311d8fe4c3735f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928540"
---
# <a name="disable-network-scan"></a>停用網路掃描

網路共用掃描可能會影響效能。  為了確保用戶端不會預設掃描網路共用/檔案，請在 Windows Defender 應用程式中將下列設定設定為 **True**：

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles