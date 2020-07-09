---
title: 所有成員都不會收到傳送到 Microsoft 365 群組的郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047230"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>所有成員都不會收到傳送到 Microsoft 365 群組的郵件

請確定所有群組成員都已訂閱，以接收電子郵件。 請參閱[追蹤 Outlook 中的群組](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)。  

若要檢查已訂閱群組電子郵件的成員的郵件狀態，請在 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps) 上執行下列命令：

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`