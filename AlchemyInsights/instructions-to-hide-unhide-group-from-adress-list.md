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
ms.openlocfilehash: 61ba34e6d554831da712a92401f26fabb02c26b7
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2020
ms.locfileid: "43908335"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a><span data-ttu-id="edf34-102">隱藏 Microsoft 365 group from address list （GAL）</span><span class="sxs-lookup"><span data-stu-id="edf34-102">Hide Microsoft 365 group from address list (GAL)</span></span>

<span data-ttu-id="edf34-103">若要從 Exchange 用戶端（例如 Outlook 或 OWA）的通訊清單（GAL）隱藏 Microsoft 365 群組，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="edf34-103">To hide an Microsoft 365 group from address lists (GAL) of Exchange clients (such as Outlook or OWA), use the following command in EXO shell:</span></span>

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

<span data-ttu-id="edf34-104">若要隱藏 Microsoft 365 群組，使其對 Exchange 用戶端無法看見，請在 EXO 命令介面中使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="edf34-104">To hide the Microsoft 365 group from being visible to Exchange clients, use the following command in EXO shell:</span></span>

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

