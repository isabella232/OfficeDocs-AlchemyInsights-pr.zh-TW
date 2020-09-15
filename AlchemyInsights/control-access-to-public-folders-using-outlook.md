---
title: 使用 Outlook 控制公用資料夾的存取權
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
- "3500007"
- "3462"
ms.openlocfilehash: 4ef62fe8c9cc438c48ed8897a8b3385b15669cdc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680483"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="26790-102">使用 Outlook 控制公用資料夾的存取權</span><span class="sxs-lookup"><span data-stu-id="26790-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="26790-103">若要控制哪些使用者能夠使用 Outlook 存取公用資料夾：</span><span class="sxs-lookup"><span data-stu-id="26790-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="26790-104">使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="26790-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="26790-105">$true：允許使用者在 Outlook 中存取公用資料夾</span><span class="sxs-lookup"><span data-stu-id="26790-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="26790-106">$false：避免使用者在 Outlook 中存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="26790-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="26790-107">這是預設值。</span><span class="sxs-lookup"><span data-stu-id="26790-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="26790-108">附注：這個程式只能用來控制 Windows 的電腦版 Outlook 用戶端連線。</span><span class="sxs-lookup"><span data-stu-id="26790-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="26790-109">使用者可以使用 OWA 或 Mac 版 Outlook 繼續存取公用資料夾。</span><span class="sxs-lookup"><span data-stu-id="26790-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="26790-110">如需詳細資訊，請參閱 [Outlook 公用資料夾的受控制連線](https://aka.ms/controlpf) 以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="26790-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
