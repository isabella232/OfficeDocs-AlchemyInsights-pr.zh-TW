---
title: 以 Microsoft 365 群組傳送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740142"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="98548-102">以 Microsoft 365 群組傳送</span><span class="sxs-lookup"><span data-stu-id="98548-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="98548-103">您可以指派 [傳送為] 權限，以允許特定使用者以 Microsoft 365 群組的方式傳送郵件：</span><span class="sxs-lookup"><span data-stu-id="98548-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="98548-104">連線至 Exchange Online PowerShell。</span><span class="sxs-lookup"><span data-stu-id="98548-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="98548-105">執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="98548-105">Run the following command:</span></span>  

    <span data-ttu-id="98548-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span><span class="sxs-lookup"><span data-stu-id="98548-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="98548-107">如需詳細資料，請參閱[允許成員使用「傳送為」或「代理傳送者」功能](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="98548-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>