---
title: 無法存取公用資料夾
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819503"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="a483d-102">Outlook 無法連接至公用資料夾</span><span class="sxs-lookup"><span data-stu-id="a483d-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="a483d-103">如果公用資料夾存取無法為某些使用者運作，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="a483d-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="a483d-104">連線至 EXO PowerShell，並在有問題的使用者帳戶上設定 DefaultPublicFolderMailbox 參數，以與使用中使用者帳戶的參數相符。</span><span class="sxs-lookup"><span data-stu-id="a483d-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="a483d-105">範例：</span><span class="sxs-lookup"><span data-stu-id="a483d-105">Example:</span></span>

<span data-ttu-id="a483d-106">Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="a483d-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="a483d-107">Set-Mailbox ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="a483d-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="a483d-108">至少等候一個小時，讓變更生效。</span><span class="sxs-lookup"><span data-stu-id="a483d-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="a483d-109">如果問題仍然存在， [請執行下列程式，以](https://aka.ms/pfcte) 使用 Outlook 疑難排解公用資料夾存取問題。</span><span class="sxs-lookup"><span data-stu-id="a483d-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="a483d-110">**若要控制哪些使用者可以使用 Outlook 存取公用資料夾**：</span><span class="sxs-lookup"><span data-stu-id="a483d-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="a483d-111">使用 Set-CASMailbox <mailboxname> PublicFolderClientAccess $true 或 $false</span><span class="sxs-lookup"><span data-stu-id="a483d-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="a483d-112">$true：允許使用者在 Outlook 中存取公用資料夾</span><span class="sxs-lookup"><span data-stu-id="a483d-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="a483d-113">$false：避免使用者在 Outlook 中存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="a483d-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="a483d-114">這是預設值。</span><span class="sxs-lookup"><span data-stu-id="a483d-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="a483d-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="a483d-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="a483d-116">**記事** 此程式只能控制 Outlook desktop for Windows 用戶端的連線。</span><span class="sxs-lookup"><span data-stu-id="a483d-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="a483d-117">使用者可以繼續使用 OWA 或 Outlook for Mac 來存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="a483d-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="a483d-118">如需詳細資訊，請參閱 [宣佈對 Outlook 中公用資料夾的可控連線支援](https://aka.ms/controlpf)。</span><span class="sxs-lookup"><span data-stu-id="a483d-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>