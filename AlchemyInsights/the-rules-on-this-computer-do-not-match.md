---
title: 錯誤：此電腦上的規則不符合
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/09/2020
ms.locfileid: "44617958"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>錯誤：此電腦上的規則不符合

若要查看此已知問題的更新狀態，請參閱[此電腦上的規則與 Microsoft Exchange 上](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)的規則不符

Outlook 小組已在組建12928.10000 中實施修正。 此修正已在內幕人士內快速，並會在2020年6月晚移至每月通道。 當您有固定的組建之後，您可能會看到 [您想要保留哪個規則？] 最後一次的提示。 出現提示時選擇 [伺服器]，然後傳回 Outlook，然後重新啟用已停用的任何規則。

在提供修正程式之前，請使用下列解決方法：

**解決方法**：在最近的報告中，發生在 Outlook desktop 中僅已建立用戶端規則的問題。 若繼續遇到問題，請考慮刪除規則，然後在 OWA （Outlook Web App）中僅建立和編輯規則，直到問題解決為止。

如果您無法手動刪除規則，您可以在啟動 outlook 時執行 outlook 命令，方法是執行/cleanrules。 這會刪除用戶端和伺服器規則。 它會刪除 Outlook 設定檔中所有帳戶的所有規則。 此命令會在命令列參數文章中進一步記載。