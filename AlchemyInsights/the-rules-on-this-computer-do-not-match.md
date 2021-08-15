---
title: 錯誤：此電腦上的規則不符合
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981104"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>錯誤：此電腦上的規則不符合

若要查看此已知問題的更新狀態，請參閱[此電腦上的規則不符合 Microsoft Exchange 的規則](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)

Outlook 小組已在組建12928.10000 中實施修正。 此修正已在內幕人士內快速，並會在2020年6月晚移至每月通道。 當您有固定的組建之後，您可能會看到 [您想要保留哪個規則？] 最後一次的提示。 出現提示時選擇 [伺服器]，然後回到 Outlook，然後重新啟用已停用的任何規則。

在提供修正程式之前，請使用下列解決方法：

**解決方法**：在最近的報告中，發生在 Outlook 桌面中已建立用戶端規則的問題。 若繼續遇到問題，請考慮刪除規則，然後只在 OWA (Outlook Web App) 中建立和編輯規則，直到問題解決為止。

如果您無法手動刪除規則，您可以在啟動 Outlook.exe/cleanrules. 時執行 Outlook 命令 Outlook 這會刪除用戶端和伺服器規則。 它會刪除 Outlook 設定檔中所有帳戶的所有規則。 此命令會在命令列參數文章中進一步記載。

