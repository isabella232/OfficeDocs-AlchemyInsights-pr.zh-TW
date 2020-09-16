---
title: Exchange Online PowerShell 中的微延遲或節流
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 55844747be27ea4ff8f538492e576195b3a5f0bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47743904"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Exchange Online PowerShell 中的微延遲或節流

在 Exchange Online 中執行指令碼和 Cmdlet 時，您可能會看到「已套用微延遲」警告或延遲。 以下是兩個相關建議：

- 您可以嘗試使用 [Exchange Online v2 PowerShell 模組](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps)，其中包含以 REST API 為基礎的 Cmdlet，且效能更加顯著。 這可能是許多常用 Get- Cmdlet 的絕佳解決方案。
- 如果您需要使用 v2 模組中尚未涵蓋的 Cmdlet，請參閱[在 Office 365 中為大量使用者執行 PowerShell Cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)，其討論如何在 Exchange Online 中避免預期的 PowerShell 節流限制。
