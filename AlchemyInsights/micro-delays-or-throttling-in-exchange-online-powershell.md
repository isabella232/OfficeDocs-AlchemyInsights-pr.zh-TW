---
title: Exchange Online PowerShell 中的微延遲或節流
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: cb97aa790264c23aae15fed49c353c7fb0d6209d9492c6881f1b1091fe80d7b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57868525"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell 中的微延遲或節流

在 Exchange Online 中執行指令碼和 Cmdlet 時，您可能會看到「已套用微延遲」警告或延遲。 以下是一些如何解決此問題的建議：

- 請執行我們的診斷以放寬租用戶的 PowerShell 節流原則。 此解決方案可解決大部分的問題。
- 如果問題仍未解決，請使用 [Exchange Online v2 PowerShell 模組](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)，其中包含以 REST API 為基礎的 Cmdlet，且效能更加顯著。 這可能是許多常用 Get- Cmdlet 的絕佳解決方案。
- 如果您需要使用 v2 模組中未涵蓋的 Cmdlet，請參閱[在 Office 365 中為大量使用者執行 PowerShell Cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，其討論如何在 Exchange Online 中避免 PowerShell 節流限制。
