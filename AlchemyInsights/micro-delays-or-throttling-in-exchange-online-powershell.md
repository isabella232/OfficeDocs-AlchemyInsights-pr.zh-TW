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
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830024"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell 中的微延遲或節流

在 Exchange Online 中執行指令碼和 Cmdlet 時，您可能會看到「已套用微延遲」警告或延遲。 以下是兩個相關建議：

- 您可以嘗試使用 [Exchange Online v2 PowerShell 模組](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)，其中包含以 REST API 為基礎的 Cmdlet，且效能更加顯著。 這可能是許多常用 Get- Cmdlet 的絕佳解決方案。
- 如果您需要使用 v2 模組中尚未涵蓋的 Cmdlet，請參閱[在 Office 365 中為大量使用者執行 PowerShell Cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，其討論如何在 Exchange Online 中避免預期的 PowerShell 節流限制。
