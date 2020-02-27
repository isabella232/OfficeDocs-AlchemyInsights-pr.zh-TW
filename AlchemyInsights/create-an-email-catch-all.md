---
title: 建立電子郵件全部
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286060"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="764e2-102">建立電子郵件全部</span><span class="sxs-lookup"><span data-stu-id="764e2-102">Create an email catch all</span></span>

<span data-ttu-id="764e2-103">使用的全部是強烈建議不要。</span><span class="sxs-lookup"><span data-stu-id="764e2-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="764e2-104">最好是提供退回回給您，讓寄件者知道為解決讓他們可以採取的動作無法傳遞郵件寄件者。</span><span class="sxs-lookup"><span data-stu-id="764e2-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="764e2-105">您也可以限制為僅限以前有效的電子郵件地址受監視的信箱。</span><span class="sxs-lookup"><span data-stu-id="764e2-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="764e2-106">任何全部信箱將會收到了很多垃圾郵件，並可能最終填滿，如果不密切監視。</span><span class="sxs-lookup"><span data-stu-id="764e2-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="764e2-107">（還有接收限制）。</span><span class="sxs-lookup"><span data-stu-id="764e2-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="764e2-108">如果您決定要繼續，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="764e2-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="764e2-109">建立動態通訊群組 & 包含 「 所有收件者類型 >。</span><span class="sxs-lookup"><span data-stu-id="764e2-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="764e2-110">建立專用的信箱來捕捉電子郵件，例如 catchall@domain.com。</span><span class="sxs-lookup"><span data-stu-id="764e2-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="764e2-111">為特定網域，設定 「 InternalRelay 」 至 DomainType。</span><span class="sxs-lookup"><span data-stu-id="764e2-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="764e2-112">如果您稍後移除全部，請務必設定為 [授權網域。</span><span class="sxs-lookup"><span data-stu-id="764e2-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="764e2-113">建立郵件流程傳輸規則，如下所示：</span><span class="sxs-lookup"><span data-stu-id="764e2-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="764e2-114">如果寄件者為 「 外部組織 」</span><span class="sxs-lookup"><span data-stu-id="764e2-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="764e2-115">將郵件重新導向至 Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="764e2-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="764e2-116">除非收件者屬於的 allusers@domain.com （通訊群組包含所有成員）</span><span class="sxs-lookup"><span data-stu-id="764e2-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="764e2-117">確保以驗證新的信箱會新增至動態通訊群組</span><span class="sxs-lookup"><span data-stu-id="764e2-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
