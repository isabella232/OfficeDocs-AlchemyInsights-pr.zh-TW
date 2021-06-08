---
title: Linux 上適用於端點的 Microsoft Defender 效能問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783422"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Linux 上適用於端點的 Microsoft Defender 效能問題

本文引導您完成識別 Linux 上適用於端點的 Microsoft Defender 效能問題的步驟。

重要的是，要先驗證您遇到的問題是使用 [最新版本](/microsoft-365/security/defender-endpoint/linux-whatsnew) 解決的。 

若要啟動您的調查，請參閱 [疑難排解 Linux 上適用於端點的 Microsoft Defender 效能問題](/microsoft-365/security/defender-endpoint/linux-support-perf)。

## <a name="exclusions"></a>排除項目

排除項目可以協助降低效能問題。 在您開始之前先檢視您的排除項目，以得知任何其他風險並紀錄之。

如需詳細資訊，請參閱[設定及驗證 Linux 上適用於端點的 Microsoft Defender 排除項目](/microsoft-365/security/defender-endpoint/linux-exclusions)。

當您有多個位於相同掛接點的檔案和資料夾要進行排除時，在掛接點進行排除可能更為容易。 從二月份發行版本 101.22.80 開始，您可以排除整個掛接點。

例如，如果 /mnt/backup 是一個掛接點，您可以透過執行此命令，將 /mnt/backup 新增至排除清單：

`$ mdatp exclusion folder add –path /mnt/backup`

**注意**：新增排除項目會增加無法偵測的惡意程式碼風險，且應小心處置和執行。

## <a name="need-help"></a>需要協助嗎？

若要以最有效的方式協助您，請在開啟支援案例之前，收集診斷資料。
