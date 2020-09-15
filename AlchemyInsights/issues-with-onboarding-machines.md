---
title: 電腦上線的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676873"
---
# <a name="issues-with-onboarding-machines"></a>電腦上線的問題

將電腦上線到 MDATP 服務時，您可能會遇到問題。 若您想要存取終端使用者的電腦，請依照下列步驟操作：

1. 下載 [用戶端連線分析程式](https://aka.ms/mdatpanalyzer) 診斷工具。
2. 解壓縮並執行 MDATPAnalyzer.cmd 指令。
3. 在名為 MDATPClientAnalyzerResult 的資料夾（用於下載分析器工具的同個資料夾 ）中找到 [診斷記錄]。
4. 檢視記錄檔 MDATPClientAnalyzer.txt 並用以查找連線或網際網路 proxy 設定問題。