---
title: 輸出轉送集區
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/08/2021
ms.locfileid: "53339957"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="fc999-102">輸出轉送集區</span><span class="sxs-lookup"><span data-stu-id="fc999-102">Outbound relay pool</span></span>

<span data-ttu-id="fc999-103">Microsoft 正在對設定進行一些變更，以透過 Microsoft 365 轉送或轉寄電子郵件。</span><span class="sxs-lookup"><span data-stu-id="fc999-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="fc999-104">特定案例中的郵件會透過 Microsoft 365 使用特殊轉送集區轉寄或轉送。</span><span class="sxs-lookup"><span data-stu-id="fc999-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="fc999-105">使用轉送集區傳送的郵件會在收件者的 [垃圾郵件] 資料夾中結束。</span><span class="sxs-lookup"><span data-stu-id="fc999-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="fc999-106">如需詳細資訊，請參閱[輸出傳遞](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)集區</span><span class="sxs-lookup"><span data-stu-id="fc999-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="fc999-107">若要避免使用轉送集區的情況，請確定轉寄/轉送郵件符合下列其中一個條件：</span><span class="sxs-lookup"><span data-stu-id="fc999-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="fc999-108">輸出寄件者是租使用者的網域。</span><span class="sxs-lookup"><span data-stu-id="fc999-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="fc999-109">當郵件 Microsoft 365 時，寄件者原則框架 (SPF) 傳送。</span><span class="sxs-lookup"><span data-stu-id="fc999-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="fc999-110">當郵件到達 Microsoft 365 時，DomainKeys 身分識別的郵件 (DKIM) 在 P2 寄件者網域上傳遞。</span><span class="sxs-lookup"><span data-stu-id="fc999-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="fc999-111">符合上述準則的郵件不會透過轉送集區中繼。</span><span class="sxs-lookup"><span data-stu-id="fc999-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="fc999-112">如果您網域的 MX 記錄指向協力廠商或內部部署伺服器，請使用增強型篩選，以確定輸入電子郵件的 SPF 驗證是否正確，以及避免透過轉送集區傳送電子郵件。</span><span class="sxs-lookup"><span data-stu-id="fc999-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="fc999-113">**如何判斷我們是否受到轉送集區的影響？**</span><span class="sxs-lookup"><span data-stu-id="fc999-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="fc999-114">如果轉寄或轉送的電子郵件使用上述其中一個條件，則郵件將不會透過轉送集區中繼。</span><span class="sxs-lookup"><span data-stu-id="fc999-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="fc999-115">不過，如果透過轉送集區傳送郵件，則輸出伺服器 IP 是在 40.95.0.0/16 範圍內，而外寄伺服器名稱則包含 **rly** 的名稱。</span><span class="sxs-lookup"><span data-stu-id="fc999-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

