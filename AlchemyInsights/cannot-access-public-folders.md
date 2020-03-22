---
title: 無法存取公用資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891740"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="7e904-102">Outlook 無法連接至公用資料夾</span><span class="sxs-lookup"><span data-stu-id="7e904-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="7e904-103">如果公用資料夾存取無法為某些使用者運作，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="7e904-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="7e904-104">連線至 EXO PowerShell，並在有問題的使用者帳戶上設定 DefaultPublicFolderMailbox 參數，以與使用中使用者帳戶的參數相符。</span><span class="sxs-lookup"><span data-stu-id="7e904-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="7e904-105">範例：</span><span class="sxs-lookup"><span data-stu-id="7e904-105">Example:</span></span>

<span data-ttu-id="7e904-106">Get-Mailbox WorkingUser |ft DefaultPublicFolderMailbox，EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="7e904-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="7e904-107">Set-Mailbox 來自上一個\<命令的 ProblemUser-DefaultPublicFolderMailbox 值></span><span class="sxs-lookup"><span data-stu-id="7e904-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="7e904-108">至少等候一個小時，讓變更生效。</span><span class="sxs-lookup"><span data-stu-id="7e904-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="7e904-109">如果問題仍然存在，[請執行下列程式，以](https://aka.ms/pfcte)使用 Outlook 疑難排解公用資料夾存取問題。</span><span class="sxs-lookup"><span data-stu-id="7e904-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>