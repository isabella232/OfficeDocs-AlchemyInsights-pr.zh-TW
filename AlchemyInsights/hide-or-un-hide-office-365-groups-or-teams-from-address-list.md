---
title: 從通訊清單隱藏或取消隱藏 Office 365 群組或小組
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
- "9002947"
- "5642"
ms.openlocfilehash: 1204b9f45fe34015f72c559f77674e980d28c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47782318"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>從通訊清單隱藏或取消隱藏 Office 365 群組或小組

使用下列 EXO PowerShell 命令來隱藏或取消隱藏 Exchange 用戶端 (Outlook、OWA) 通訊清單 (GAL) 中的 Office 365 群組/小組：

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

使用下列 EXO PowerShell 命令來隱藏或取消隱藏 Exchange 用戶端 (Outlook、OWA) 中的 Office365 群組/小組：

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- 如需詳細指示，請參閱[隱藏 GAL 和 Exchange 用戶端中的 Office 365 群組](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)。
