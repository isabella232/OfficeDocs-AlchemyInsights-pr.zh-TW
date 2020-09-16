---
title: 將 PowerShell 指令碼連線到 Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 3a8383a57bc1267311daf03c78841070cca8fb8f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748055"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="4c805-102">將 PowerShell 指令碼連線到 Exchange Online</span><span class="sxs-lookup"><span data-stu-id="4c805-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="4c805-103">Exchange Online 中的基本驗證即將淘汰，之後的方式是使用指令碼和自動工作的認證驗證。</span><span class="sxs-lookup"><span data-stu-id="4c805-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="4c805-104">若要深入了解，請參閱 [EXO V2 模組中，自動指令碼的僅應用程式驗證](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2)。</span><span class="sxs-lookup"><span data-stu-id="4c805-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>