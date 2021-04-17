---
title: 在通訊清單中隱藏/取消隱藏群組的指示
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 4d55866700b9b8494f1f692cd3b865116b96a1bc
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831869"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="e9c72-102">從通訊清單中隱藏 Microsoft 365 群組 (GAL) </span><span class="sxs-lookup"><span data-stu-id="e9c72-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="e9c72-103">若要從 Exchange 用戶端 (（如 Outlook 或 OWA) ）的通訊清單 (GAL) 中隱藏 Microsoft 365 群組，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="e9c72-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="e9c72-104">若要隱藏 Microsoft 365 群組，使其對 Exchange 用戶端無法看見，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="e9c72-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

