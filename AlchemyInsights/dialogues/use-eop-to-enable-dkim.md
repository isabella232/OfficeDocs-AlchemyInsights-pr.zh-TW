---
title: 使用 Exchange Online PowerShell 啟用特定網域的 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50500740"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="ad379-102">使用 Exchange Online PowerShell 啟用特定網域的 DKIM</span><span class="sxs-lookup"><span data-stu-id="ad379-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="ad379-103">如果您無法在系統管理中心建立 DKIM DNS 記錄，請嘗試使用 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="ad379-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="ad379-104">若要使用 Exchange Online PowerShell 建立 DKIM DNS 記錄，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="ad379-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="ad379-105">以系統管理員身分開啟 Windows PowerShell，並在所述的順序中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="ad379-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="ad379-106">a.</span><span class="sxs-lookup"><span data-stu-id="ad379-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="ad379-107">b.</span><span class="sxs-lookup"><span data-stu-id="ad379-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="ad379-108">c.</span><span class="sxs-lookup"><span data-stu-id="ad379-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="ad379-109">如果您無法連線至 Exchange Online PowerShell，請參閱 [Connect To Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)。</span><span class="sxs-lookup"><span data-stu-id="ad379-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="ad379-110">當您連線至 Exchange Online PowerShell 後，請執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="ad379-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="ad379-111">在成功執行上述命令之後，請執行下列命令終止 Exchange Online PowerShell 會話：</span><span class="sxs-lookup"><span data-stu-id="ad379-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



