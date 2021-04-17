---
title: 使用 Outlook 控制公用資料夾的存取權
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816731"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="0ed73-102">使用 Outlook 控制公用資料夾的存取權</span><span class="sxs-lookup"><span data-stu-id="0ed73-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="0ed73-103">若要控制哪些使用者能夠使用 Outlook 存取公用資料夾：</span><span class="sxs-lookup"><span data-stu-id="0ed73-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="0ed73-104">使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="0ed73-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="0ed73-105">$true：允許使用者在 Outlook 中存取公用資料夾</span><span class="sxs-lookup"><span data-stu-id="0ed73-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="0ed73-106">$false：避免使用者在 Outlook 中存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="0ed73-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="0ed73-107">這是預設值。</span><span class="sxs-lookup"><span data-stu-id="0ed73-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="0ed73-108">附注：這個程式只能用來控制 Windows 的電腦版 Outlook 用戶端連線。</span><span class="sxs-lookup"><span data-stu-id="0ed73-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="0ed73-109">使用者可以使用 OWA 或 Mac 版 Outlook 繼續存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="0ed73-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="0ed73-110">如需詳細資訊，請參閱 [Outlook 公用資料夾的受控制連線](https://aka.ms/controlpf) 以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="0ed73-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
