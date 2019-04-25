---
title: 1332 OWA 位收件匣規則都不執行信箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372551"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="ef01b-102">收件匣規則不會如預期般運作</span><span class="sxs-lookup"><span data-stu-id="ef01b-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="ef01b-103">確認下列設定：</span><span class="sxs-lookup"><span data-stu-id="ef01b-103">Verify the following settings:</span></span>

- <span data-ttu-id="ef01b-104">郵件可以重新導向、 轉寄或回覆自動根據收件匣規則僅一次。</span><span class="sxs-lookup"><span data-stu-id="ef01b-104">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time.</span></span> <span data-ttu-id="ef01b-105">重新導向規則 （收件匣規則或郵件流程規則，也稱為傳輸規則） 可以將最大值為十個轉寄收件者新增至郵件。</span><span class="sxs-lookup"><span data-stu-id="ef01b-105">A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message.</span></span> <span data-ttu-id="ef01b-106">如需詳細資訊，請參閱[日誌、 傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="ef01b-106">For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>

- <span data-ttu-id="ef01b-107">收件匣規則不替代日誌記錄信箱上運作。</span><span class="sxs-lookup"><span data-stu-id="ef01b-107">Inbox rules don't work on the alternate journaling mailbox.</span></span> <span data-ttu-id="ef01b-108">如需替代日誌記錄信箱的詳細資訊，請參閱 <<c0>替代日誌記錄信箱。</span><span class="sxs-lookup"><span data-stu-id="ef01b-108">For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>

<span data-ttu-id="ef01b-109">若要修正這些問題，請參閱 < <b0>KB 2829319</b0>。</span><span class="sxs-lookup"><span data-stu-id="ef01b-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>

<span data-ttu-id="ef01b-110">如果不套用先前的問題，請向上呈報給 Microsoft 支援服務問題之前執行收件匣規則診斷報告：</span><span class="sxs-lookup"><span data-stu-id="ef01b-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>

1. <span data-ttu-id="ef01b-111">在網頁型 Outlook 中開啟信箱，然後按一下 [**設定** \> **選項** \> **組合管理電子郵件** \> **收件匣規則**。</span><span class="sxs-lookup"><span data-stu-id="ef01b-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>

2. <span data-ttu-id="ef01b-112">在頁面底部，按一下 [**您的規則如果無法使用 [按一下這裡以產生診斷報告**]。</span><span class="sxs-lookup"><span data-stu-id="ef01b-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
