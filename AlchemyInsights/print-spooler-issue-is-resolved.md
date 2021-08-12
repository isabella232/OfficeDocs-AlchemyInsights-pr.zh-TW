---
title: 已解決列印多工緩衝處理器問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/8/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5151"
- "9002659"
ms.openlocfilehash: 73ff86928c043dd41f49d456d30c2fcf7947bd4cb304d0456c634d4fa5808239
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911329"
---
# <a name="print-spooler-issue-is-resolved"></a>已解決列印多工緩衝處理器問題

如果您的裝置更新為 Windows 10 **作業系統組建 19041.329**，您可能會發現特定印表機無法列印的問題。 列印多工緩衝處理器可能會在嘗試列印時發生錯誤或意外關閉，且受影響的印表機不會有任何輸出。 此問題已在作業系統組建 **19041.331**、[KB4567523](https://support.microsoft.com/help/4567523/windows-10-update-kb4567523) 中解決。  

**持續調查**

在部分裝置上，本機安全性授權子系統服務 (LSASS) 檔案 (**Isass.exe**) 可能會失敗，並顯示以下錯誤訊息：「重要系統處理序 C:\WINDOWS\system32\Isass.exe 失敗，狀態碼為 c0000008。 電腦現在必須重新開機」。  **Microsoft 正努力研究解決方法，並會在即將推出的版本中提供更新。**

如需詳細資訊，請參閱 [Windows 10 版本 2004 已知問題](https://docs.microsoft.com/windows/release-information/status-windows-10-2004#442msgdesc)。