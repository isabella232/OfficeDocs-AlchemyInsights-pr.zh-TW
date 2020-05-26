---
title: Microsoft 365 群組中的歡迎訊息
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "5685"
ms.openlocfilehash: d82931ae6978a09e674b00640d1dd413bcce7cfd
ms.sourcegitcommit: b196100759b29aecd62b693a2bfedbbd25a697c6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2020
ms.locfileid: "44320451"
---
# <a name="welcome-message-in-microsoft-365-groups"></a>Microsoft 365 群組中的歡迎訊息

如果 "UnifiedGroupWelcomeMessageEnabled" 屬性為 True，則加入 Microsoft 365 群組的新使用者將會收到歡迎電子郵件。

若要停用歡迎訊息，請使用下列 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 命令：

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
