---
title: 從通訊清單隱藏或取消隱藏 Office 365 群組或小組
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
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088387"
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
