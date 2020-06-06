---
title: 在通訊清單中隱藏/取消隱藏群組的指示
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580000"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="0afc6-102">隱藏 Microsoft 365 group from address list （GAL）</span><span class="sxs-lookup"><span data-stu-id="0afc6-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="0afc6-103">若要隱藏 Exchange 用戶端（例如 Outlook 或 OWA）的通訊清單（GAL）中的 Microsoft 365 群組，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="0afc6-103">To hide a Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="0afc6-104">若要隱藏 Microsoft 365 群組，使其對 Exchange 用戶端無法看見，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="0afc6-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

