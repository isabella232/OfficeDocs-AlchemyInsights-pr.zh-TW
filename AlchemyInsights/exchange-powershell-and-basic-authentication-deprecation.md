---
title: Exchange PowerShell 和基本驗證取代
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: a0f01d7ecaa444777aa0675795e588790ab22f19
ms.sourcegitcommit: 9e44b852d18a2816acac0aacb78cb99b4c114368
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "45205186"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="6f4d9-102">Exchange PowerShell 和基本驗證取代</span><span class="sxs-lookup"><span data-stu-id="6f4d9-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="6f4d9-103">如需在不使用基本驗證的情況下連線至 Exchange Online PowerShell 方法的相關最新資訊，請 [移至此處](https://aka.ms/exops-docs)。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="6f4d9-104">PowerShell V2 模組不使用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="6f4d9-105">請注意，您的用戶端電腦仍需啟用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="6f4d9-106">新版 PowerShell V2 模組會使用新式驗證來建立啟用所有 REST 基礎 V2 Cmdlet 的連線。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="6f4d9-107">除了 V2 Cmdlet 以外，它也可讓您存取需要建立遠端 PowerShell 工作階段的舊版遠端 PowerShell (RPS) Cmdlets。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="6f4d9-108">即使模組使用新式驗證機制來驗證服務，在 Windows 電腦上建立 RPS 工作階段需要在用戶端電腦上啟用 WinRM 基本驗證。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="6f4d9-109">WinRM 基本驗證管線是用來傳輸新式驗證權杖。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="6f4d9-110">如果在用戶端電腦上停用WinRM 基本驗證，新版 V2 Cmdlet 將繼續運作 (但舊版 RPS 不會)。</span><span class="sxs-lookup"><span data-stu-id="6f4d9-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
