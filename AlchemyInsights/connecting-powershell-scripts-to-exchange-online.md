---
title: 將 PowerShell 指令碼連線到 Exchange Online
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6069"
- "3500011"
ms.openlocfilehash: 34301e62a25e11c5d4c353166f8208ef74245dfa
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205390"
---
# <a name="connecting-powershell-scripts-to-exchange-online"></a><span data-ttu-id="a01a4-102">將 PowerShell 指令碼連線到 Exchange Online</span><span class="sxs-lookup"><span data-stu-id="a01a4-102">Connecting PowerShell scripts to Exchange Online</span></span>

<span data-ttu-id="a01a4-103">Exchange Online 中的基本驗證即將淘汰，之後的方式是使用指令碼和自動工作的認證驗證。</span><span class="sxs-lookup"><span data-stu-id="a01a4-103">Basic Authentication in Exchange Online is going to be deprecated, and the way forward is to connect by using certificate-based authentication for scripts and unattended tasks.</span></span> <span data-ttu-id="a01a4-104">若要深入了解，請參閱 [EXO V2 模組中，自動指令碼的僅應用程式驗證](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2)。</span><span class="sxs-lookup"><span data-stu-id="a01a4-104">To learn more, see [App-only authentication for unattended scripts in the EXO V2 module](https://docs.microsoft.com/powershell/exchange/app-only-auth-powershell-v2).</span></span>