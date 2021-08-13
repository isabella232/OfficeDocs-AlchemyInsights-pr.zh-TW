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
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926236"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>從通訊清單中隱藏 Microsoft 365 群組 (GAL) 

若要從通訊清單中隱藏 Microsoft 365 群組 (GAL) 為 Exchange 用戶端 (例如 Outlook 或 OWA) ，請在 EXO 命令介面中使用下列命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隱藏 Microsoft 365 群組，使其無法在 Exchange 用戶端看見，請在 EXO 命令介面中使用下列命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

