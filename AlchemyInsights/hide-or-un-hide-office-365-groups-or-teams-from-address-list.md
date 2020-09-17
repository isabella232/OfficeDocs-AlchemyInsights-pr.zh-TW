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
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a><span data-ttu-id="45cd1-102">從通訊清單隱藏或取消隱藏 Office 365 群組或小組</span><span class="sxs-lookup"><span data-stu-id="45cd1-102">Hide or un-hide Office 365 groups or teams from address list</span></span>

<span data-ttu-id="45cd1-103">使用下列 EXO PowerShell 命令來隱藏或取消隱藏 Exchange 用戶端 (Outlook、OWA) 通訊清單 (GAL) 中的 Office 365 群組/小組：</span><span class="sxs-lookup"><span data-stu-id="45cd1-103">Use the following EXO PowerShell command to hide or un-hide Office 365 group/teams from address lists (GAL) of Exchange clients (Outlook, OWA):</span></span>

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

<span data-ttu-id="45cd1-104">使用下列 EXO PowerShell 命令來隱藏或取消隱藏 Exchange 用戶端 (Outlook、OWA) 中的 Office365 群組/小組：</span><span class="sxs-lookup"><span data-stu-id="45cd1-104">Use the following EXO PowerShell command to hide or un-hide the Office365 group/teams from Exchange clients (Outlook, OWA):</span></span>

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- <span data-ttu-id="45cd1-105">如需詳細指示，請參閱[隱藏 GAL 和 Exchange 用戶端中的 Office 365 群組](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)。</span><span class="sxs-lookup"><span data-stu-id="45cd1-105">For detailed instructions, see [Hide Office 365 Groups from the GAL and Exchange Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).</span></span>
