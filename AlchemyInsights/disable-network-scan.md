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
ms.openlocfilehash: 7b0f5c21a7e6afda0ee3000e75ee725cbadcedb7
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449067"
---
# <a name="disable-network-scan"></a>停用網路掃描

網路共用掃描可能會影響效能。  為了確保用戶端不會預設掃描網路共用/檔案，請將 Windows Defender 應用程式中的下列設定設定為 **True**：

- DisableScanningMappedNetworkDrivesForFullScan
- DisableScanningNetworkFiles