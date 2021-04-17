---
title: 需要有關電子郵件傳送限制的協助嗎？
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836270"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="41f20-102">需要有關電子郵件傳送限制的協助嗎？</span><span class="sxs-lookup"><span data-stu-id="41f20-102">Need help with email sending limits?</span></span>

<span data-ttu-id="41f20-103">以下是服務強制執行的 **預設傳送限制**。</span><span class="sxs-lookup"><span data-stu-id="41f20-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="41f20-104">這些限制的詳細資訊記載在[這裡](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)。</span><span class="sxs-lookup"><span data-stu-id="41f20-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="41f20-105">若要防止傳送未經授權的大宗郵件，我們會為每位使用者套用 **所有傳出和內部郵件的收件人比率限制**。</span><span class="sxs-lookup"><span data-stu-id="41f20-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="41f20-106">在所有 SKU 中，此限制為每天 **10,000 位收件者**。</span><span class="sxs-lookup"><span data-stu-id="41f20-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="41f20-107">客戶若需要傳送合法的大量商業電子郵件 (例如客戶電子報)，應使用專門提供這些服務的第三方供應商。</span><span class="sxs-lookup"><span data-stu-id="41f20-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="41f20-108">**注意**：達到收件人比率限制之後，就無法從信箱傳送郵件，除非收到郵件的收件者人數在過去 24 小時內減少到上限範圍內。</span><span class="sxs-lookup"><span data-stu-id="41f20-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="41f20-109">在那之前，使用者將無法傳送郵件。</span><span class="sxs-lookup"><span data-stu-id="41f20-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="41f20-110">所有 SKU 都會套用 **每分鐘 30 封郵件** 的郵件比率限制。</span><span class="sxs-lookup"><span data-stu-id="41f20-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="41f20-111">這個限制決定使用者在指定時間內可從 Exchange Online 帳戶傳送的郵件數量。</span><span class="sxs-lookup"><span data-stu-id="41f20-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="41f20-112">在所有 SKU 中，**[收件者]、[副本] 和 [密件副本]欄位允許的收件者數量上限** 是 **1000 位收件人**。</span><span class="sxs-lookup"><span data-stu-id="41f20-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="41f20-113">若要自訂這個限制，請移至[這裡](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)。</span><span class="sxs-lookup"><span data-stu-id="41f20-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
