---
title: Microsoft 365 群組中的歡迎訊息
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
- "1200024"
- "5685"
ms.openlocfilehash: de16ca6021441bf6cb781106b7f3da8eed86b0f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725830"
---
# <a name="welcome-message-in-microsoft-365-groups"></a><span data-ttu-id="228f2-102">Microsoft 365 群組中的歡迎訊息</span><span class="sxs-lookup"><span data-stu-id="228f2-102">Welcome message in Microsoft 365 Groups</span></span>

<span data-ttu-id="228f2-103">如果 "UnifiedGroupWelcomeMessageEnabled" 屬性為 True，則加入 Microsoft 365 群組的新使用者將會收到歡迎電子郵件。</span><span class="sxs-lookup"><span data-stu-id="228f2-103">New users joining Microsoft 365 group will receive welcome email if the "UnifiedGroupWelcomeMessageEnabled" property is True.</span></span>

<span data-ttu-id="228f2-104">若要停用歡迎訊息，請使用下列 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) 命令：</span><span class="sxs-lookup"><span data-stu-id="228f2-104">In case you want to disable the welcome message, use the following [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) command:</span></span>

`
Set-UnifiedGroup <groupname> -UnifiedGroupWelcomeMessageEnabled:$False
`
