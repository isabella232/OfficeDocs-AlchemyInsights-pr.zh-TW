---
title: 在通訊清單中隱藏/取消隱藏群組的指示
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663000"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>從通訊清單中隱藏 Microsoft 365 群組 (GAL) 

若要從 Exchange 用戶端 (（如 Outlook 或 OWA) ）的通訊清單 (GAL) 中隱藏 Microsoft 365 群組，請在 EXO 命令介面中使用下列命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隱藏 Microsoft 365 群組，使其對 Exchange 用戶端無法看見，請在 EXO 命令介面中使用下列命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

