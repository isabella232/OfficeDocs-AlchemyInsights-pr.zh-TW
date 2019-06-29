---
title: 1332 OWA-收件匣規則未執行信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360908"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="5ce24-102">收件匣規則無法如預期般運作</span><span class="sxs-lookup"><span data-stu-id="5ce24-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="5ce24-103">確認下列設定:</span><span class="sxs-lookup"><span data-stu-id="5ce24-103">Verify the following settings:</span></span>

- <span data-ttu-id="5ce24-104">只能根據收件匣規則, 自動重新導向、轉寄或回復郵件一次。</span><span class="sxs-lookup"><span data-stu-id="5ce24-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="5ce24-105">重新導向規則 (收件匣規則或郵件流程規則, 也稱為傳輸規則) 最多可以新增十個轉寄收件者給郵件。</span><span class="sxs-lookup"><span data-stu-id="5ce24-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="5ce24-106">如需詳細資訊, 請參閱[日誌、傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="5ce24-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="5ce24-107">收件匣規則無法在替代日誌記錄信箱上運作。</span><span class="sxs-lookup"><span data-stu-id="5ce24-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="5ce24-108">如需替代日誌記錄信箱的詳細資訊, 請參閱[替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="5ce24-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="5ce24-109">若要修正這些問題, 請參閱[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="5ce24-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="5ce24-110">如果未套用先前的問題, 請先執行收件匣規則診斷報告, 再將問題升級至 Microsoft 支援:</span><span class="sxs-lookup"><span data-stu-id="5ce24-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="5ce24-111">在網頁版 Outlook 中開啟信箱, 然後按一下 [**設定** \> **選項** \> ] [**組織電子郵件** \> **收件匣規則**]。</span><span class="sxs-lookup"><span data-stu-id="5ce24-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="5ce24-112">在頁面底部, 按一下 [**如果您的規則未運作], 請按一下此處產生診斷報告**。</span><span class="sxs-lookup"><span data-stu-id="5ce24-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
