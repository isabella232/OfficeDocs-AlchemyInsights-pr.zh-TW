---
title: 需要將網域或電子郵件寄件者標示為安全嗎？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281127"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="67c70-102">需要將網域或電子郵件寄件者標示為安全嗎？</span><span class="sxs-lookup"><span data-stu-id="67c70-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="67c70-103">我們**不建議使用安全寄件者清單**，因為這會將組織暴露在垃圾郵件、網路釣魚詐騙和詐騙攻擊中。</span><span class="sxs-lookup"><span data-stu-id="67c70-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="67c70-104">不過，如果有業務需求，我們**建議**使用**[郵件流程規則](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。</span><span class="sxs-lookup"><span data-stu-id="67c70-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="67c70-105">我們的指導方針可確保寄件者驗證 (驗證送出網域未遭到假冒)。</span><span class="sxs-lookup"><span data-stu-id="67c70-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="67c70-106">**注意**：我們不建議使用安全的寄件者清單來管理誤判，因為垃圾郵件篩選的例外狀況可能會讓您的組織暴露在安全性攻擊中。</span><span class="sxs-lookup"><span data-stu-id="67c70-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="67c70-107">如果您的使用者收到錯誤標示為 [垃圾郵件] 的郵件，請**[向 Microsoft 回報郵件和檔案](https://protection.office.com/reportsubmission)** (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="67c70-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="67c70-108">應避免\*\*\*\* Outlook 中的安全寄件者、允許的寄件者清單或反垃圾郵件原則中的允許網域清單，因為寄件者人會繞過所有垃圾郵件、詐騙和網路魚防護以及寄件者驗證 (SPF、DKIM、DMARC)。</span><span class="sxs-lookup"><span data-stu-id="67c70-108">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC).</span></span> <span data-ttu-id="67c70-109">這個方法最適合用來進行暫時測試。</span><span class="sxs-lookup"><span data-stu-id="67c70-109">This method is best used for temporary testing only.</span></span>
