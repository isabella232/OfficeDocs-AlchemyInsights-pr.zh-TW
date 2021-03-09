---
title: 以遠端方式修正上架 Windows 10 裝置至 Microsoft Defender 高級威脅防護的問題
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529927"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>以遠端方式修正上架 Windows 10 裝置至 Microsoft Defender 高級威脅防護的問題

若您可以存取遠端電腦，請執行下列步驟：

1. 下載 [用戶端連線分析程式](https://go.microsoft.com/fwlink/?linkid=2143466) 診斷工具。
2. 解壓縮並執行 MDATPAnalyzer.cmd 指令。
3. 在 MDATPClientAnalyzerResult 資料夾中尋找診斷記錄檔，該資料夾是 Analyzer 工具下載所在的相同資料夾。
4. 若要尋找 connectivity 或網際網路 proxy 設定的問題，請複查記錄檔 MDATPClientAnalyzer.txt。

若要深入瞭解，請參閱 [電腦上架的問題](https://go.microsoft.com/fwlink/?linkid=2143634)。
