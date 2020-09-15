---
title: 建立電子郵件全部捕獲
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712977"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="1bc7c-102">建立電子郵件全部捕獲</span><span class="sxs-lookup"><span data-stu-id="1bc7c-102">Create an email catch all</span></span>

<span data-ttu-id="1bc7c-103">強烈建議使用全部捕獲。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="1bc7c-104">更好的方式是提供回復寄件者，讓寄件者知道其郵件無法依照處理方式傳遞，這樣他們才可以採取動作。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="1bc7c-105">您也可以將受監控的信箱限制為只捕捉先前有效的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="1bc7c-106">任何捕獲所有的信箱都會收到大量的垃圾郵件，而且可能會最終填滿（如果未密切監視）。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="1bc7c-107"> (有接收限制。 ) </span><span class="sxs-lookup"><span data-stu-id="1bc7c-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="1bc7c-108">如果您決定繼續，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="1bc7c-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="1bc7c-109">建立動態通訊群組 & 包括「所有收件者類型」。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="1bc7c-110">建立專用的信箱以捕捉電子郵件，例如，catchall@domain.com。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="1bc7c-111">針對特定網域，將 DomainType 設定為 "InternalRelay"。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="1bc7c-112">如果您稍後移除 [全部捕捉]，請務必將網域設回 [授權]。</span><span class="sxs-lookup"><span data-stu-id="1bc7c-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="1bc7c-113">建立郵件流程傳輸規則，如下所示：</span><span class="sxs-lookup"><span data-stu-id="1bc7c-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="1bc7c-114">如果寄件者是「組織外」</span><span class="sxs-lookup"><span data-stu-id="1bc7c-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="1bc7c-115">將郵件重新導向至 Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="1bc7c-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="1bc7c-116">除非收件者是 allusers@domain.com 的成員，否則 (通訊群組中包含所有成員) </span><span class="sxs-lookup"><span data-stu-id="1bc7c-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="1bc7c-117">確定已將新的信箱新增至動態通訊群組</span><span class="sxs-lookup"><span data-stu-id="1bc7c-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
