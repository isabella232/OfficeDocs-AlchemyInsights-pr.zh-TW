---
title: 準備在 Microsoft 365 中使用 TLS 1.2
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 1ec40ba36c69296298e24dca64a873d53682833a
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085895"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a><span data-ttu-id="7d522-102">準備在 Microsoft 365 中使用 TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="7d522-102">Prepare for use of TLS 1.2 in Microsoft 365</span></span>

<span data-ttu-id="7d522-103">從 2018 年 10 月 31 日起，Microsoft 365 將持續轉換到 TLS 1.2。</span><span class="sxs-lookup"><span data-stu-id="7d522-103">As of October 31st, 2018, Microsoft 365 will continue transitioning to TLS 1.2.</span></span> <span data-ttu-id="7d522-104">自 2020 年 10 月 15 日起，O365 將在服務中開始取代 TLS 1.0 和 1.1。</span><span class="sxs-lookup"><span data-stu-id="7d522-104">Starting October 15, 2020, O365 will begin the deprecation of TLS 1.0 and 1.1 across the service.</span></span> <span data-ttu-id="7d522-105">本次變更的推出將在未來幾周和幾個月內持續進行，但客戶應假設自 2020 年 10 月 15 日起，TLS 1.0/1.1 的服務即停止在 O365 中運作。</span><span class="sxs-lookup"><span data-stu-id="7d522-105">The rollout of this change will continue over the next few weeks and months, but customers should assume no TLS 1.0/1.1 calls will work when engaging with O365 starting Oct 15, 2020.</span></span> <span data-ttu-id="7d522-106">如前所述 (2017 年 12 月的 MC126199、2018 年 2 月的 MC128929、2019 年 7 月的 MC186827 和 2020 年 7 月的 MC218794)，我們將所有的線上服務都移至 [傳輸層安全性 (TLS)] 1.2 +，以提供頂尖的加密功能，並確保我們的服務預設為更安全。</span><span class="sxs-lookup"><span data-stu-id="7d522-106">As previously communicated (MC126199 in Dec 2017, MC128929 in Feb 2018, MC186827 in July 2019, and MC218794 in July 2020), we are moving all of our online services to Transport Layer Security (TLS) 1.2+ to provide best-in-class encryption, and to ensure our service is more secure, by default.</span></span> <span data-ttu-id="7d522-107">客戶仍可在其伺服器和資源上選擇使用 TLS 1.0/1.1，但他們應知道只有 TLS 1.2 或更新版本才能與 O365 運作。</span><span class="sxs-lookup"><span data-stu-id="7d522-107">Customers can still choose to have TLS 1.0/1.1 on their servers and resources, but they should assume only TLS 1.2 or higher will work when interacting with O365 resources.</span></span>
  
<span data-ttu-id="7d522-108">若要深入瞭解這些變更，請參閱 [此處](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) 及 [此處](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)。</span><span class="sxs-lookup"><span data-stu-id="7d522-108">To learn more about these changes, please see [here](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) and [here](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide).</span></span>

  