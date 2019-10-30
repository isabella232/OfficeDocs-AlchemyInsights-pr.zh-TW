---
title: 若要隱藏/取消隱藏群組從通訊清單的指示
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
ms.openlocfilehash: d0e0285701f1a5f308bdc682abaddf5cc2d34120
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/29/2019
ms.locfileid: "37768904"
---
# <a name="hide-office-365-group-from-address-list-gal"></a>隱藏 Office 365 群組從通訊清單 (GAL)

若要隱藏通訊清單 (GAL) 從 Office 365 群組的 Exchange 用戶端 （例如 Outlook 或 OWA），請 EXO 命令介面中使用下列命令：

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

若要隱藏防止 Exchange 用戶端看得到的 Office 365 群組，請 EXO 命令介面中使用下列命令：

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

