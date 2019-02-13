---
title: 1332 OWA 位收件匣規則未執行信箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 0d3b7ce3d6b32d94a012eb3767c0747eed80f6e5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915795"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a><span data-ttu-id="3fbff-102">收件匣規則不會在如預期般運作</span><span class="sxs-lookup"><span data-stu-id="3fbff-102">An Inbox rule doesn't work as expected</span></span>

<span data-ttu-id="3fbff-103">確認下列設定：</span><span class="sxs-lookup"><span data-stu-id="3fbff-103">Verify the following settings:</span></span>
  
- <span data-ttu-id="3fbff-p101">訊息可以重新導向、 轉寄或回覆自動根據收件匣規則只有一次。正在重新導向規則 （收件匣規則或郵件流程規則，也稱為傳輸規則） 可以新增十轉寄的收件者的最大值的郵件。如需詳細資訊，請參閱[日誌、 傳輸及收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。</span><span class="sxs-lookup"><span data-stu-id="3fbff-p101">A message can be redirected, forwarded, or replied to automatically based on Inbox rules only one time. A redirecting rule (an Inbox rule or mail flow rule, also known as a transport rule) can add a maximum of ten forwarding recipients to a message. For more information, see [Journal, Transport, and Inbox rule limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).</span></span>
    
- <span data-ttu-id="3fbff-p102">替代日誌記錄信箱不處理收件匣規則。如需備用日誌記錄信箱的詳細資訊，請參閱[替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。</span><span class="sxs-lookup"><span data-stu-id="3fbff-p102">Inbox rules don't work on the alternate journaling mailbox. For more information about the alternate journaling mailbox, see [Alternate journaling mailbox](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).</span></span>
    
<span data-ttu-id="3fbff-109">若要修正這些問題，請參閱[KB 2829319](https://support.microsoft.com/kb/2829319)。</span><span class="sxs-lookup"><span data-stu-id="3fbff-109">To fix these issues, see [KB 2829319](https://support.microsoft.com/kb/2829319).</span></span>
  
<span data-ttu-id="3fbff-110">如果未套用先前問題呈報給 Microsoft 支援問題之前執行收件匣規則診斷報告：</span><span class="sxs-lookup"><span data-stu-id="3fbff-110">If the previous issues don't apply, run the Inbox rule diagnostic report before you escalate the issue to Microsoft Support:</span></span>
  
1. <span data-ttu-id="3fbff-111">在 web 上的 Outlook 開啟信箱並按一下 [**設定** \> **選項** \> **組織電子郵件** \> **收件匣規則**。</span><span class="sxs-lookup"><span data-stu-id="3fbff-111">Open the mailbox in Outlook on the web, and click **Settings** \> **Options** \> **Organize email** \> **Inbox rules**.</span></span>
    
2. <span data-ttu-id="3fbff-112">在頁面的底端，按一下 [**如果規則無法使用 [按一下此處產生的診斷報告**。</span><span class="sxs-lookup"><span data-stu-id="3fbff-112">At the bottom of the page, click **If your rules are not working click here to generate a diagnostic report**.</span></span>
    

