---
title: 1332 OWA-收件匣規則未執行信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576551"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="24b4e-102">收件匣規則未如期運作</span><span class="sxs-lookup"><span data-stu-id="24b4e-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="24b4e-103">在 web 上的 Outlook 中確認下列設定：</span><span class="sxs-lookup"><span data-stu-id="24b4e-103">Verify the following settings in Outlook on the web:</span></span>

- <span data-ttu-id="24b4e-104">郵件只能根據收件匣規則，自動重新導向、轉寄或回復一次。</span><span class="sxs-lookup"><span data-stu-id="24b4e-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="24b4e-105">重新導向規則（收件匣規則或郵件流程規則，也稱為傳輸規則）最多可將十個轉寄收件者新增至郵件。</span><span class="sxs-lookup"><span data-stu-id="24b4e-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="24b4e-106">如需詳細資訊，請參閱[日誌、傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="24b4e-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="24b4e-107">收件匣規則不適用於替代日誌記錄信箱。</span><span class="sxs-lookup"><span data-stu-id="24b4e-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="24b4e-108">如需替代日誌記錄信箱的詳細資訊，請參閱[替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="24b4e-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="24b4e-109">若要修正這些問題，請參閱[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="24b4e-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="24b4e-110">若未套用上述問題，請先執行收件匣規則診斷報告，再將問題提升至 Microsoft 支援：</span><span class="sxs-lookup"><span data-stu-id="24b4e-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="24b4e-111">在 Outlook 網頁版中開啟信箱，然後按一下</span><span class="sxs-lookup"><span data-stu-id="24b4e-111">Open the mailbox in Outlook on the web, and click</span></span> <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 <span data-ttu-id="24b4e-112">**設定**  > **流覽所有 Outlook 設定**  > **郵件**  > **規則**。</span><span class="sxs-lookup"><span data-stu-id="24b4e-112">**Settings** > **View all Outlook Settings** > **Mail** > **Rules**.</span></span>

2. <span data-ttu-id="24b4e-113">在頁面底部，按一下 [**如果規則未正常運作]，請按一下這裡以產生診斷報告**。</span><span class="sxs-lookup"><span data-stu-id="24b4e-113">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
