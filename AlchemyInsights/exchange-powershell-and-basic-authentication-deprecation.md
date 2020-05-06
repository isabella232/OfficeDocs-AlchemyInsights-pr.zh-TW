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
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: 264b782ac2fba8ffd84524180dc4f7d60b45e9a4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/04/2020
ms.locfileid: "44015680"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="ebea1-102">Exchange PowerShell 和基本驗證取代</span><span class="sxs-lookup"><span data-stu-id="ebea1-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="ebea1-103">如需在不使用基本驗證的情況下連線至 Exchange Online PowerShell 方法的相關最新資訊，請 [移至此處](https://aka.ms/psbasicauth)。</span><span class="sxs-lookup"><span data-stu-id="ebea1-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="ebea1-104">請注意，您的用戶端電腦仍需啟用基本驗證。</span><span class="sxs-lookup"><span data-stu-id="ebea1-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="ebea1-105">新版 PowerShell V2 模組會使用新式驗證來建立啟用所有 REST 基礎 V2 Cmdlet 的連線。</span><span class="sxs-lookup"><span data-stu-id="ebea1-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="ebea1-106">除了 V2 Cmdlet 以外，它也可讓您存取需要建立遠端 PowerShell 工作階段的舊版遠端 PowerShell (RPS) Cmdlets。</span><span class="sxs-lookup"><span data-stu-id="ebea1-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="ebea1-107">即使模組使用新式驗證機制來驗證服務，在 Windows 電腦上建立 RPS 工作階段需要在用戶端電腦上啟用 WinRM 基本驗證。</span><span class="sxs-lookup"><span data-stu-id="ebea1-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="ebea1-108">WinRM 基本驗證管線是用來傳輸新式驗證權杖。</span><span class="sxs-lookup"><span data-stu-id="ebea1-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="ebea1-109">如果在用戶端電腦上停用WinRM 基本驗證，新版 V2 Cmdlet 將繼續運作 (但舊版 RPS 不會)。</span><span class="sxs-lookup"><span data-stu-id="ebea1-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
