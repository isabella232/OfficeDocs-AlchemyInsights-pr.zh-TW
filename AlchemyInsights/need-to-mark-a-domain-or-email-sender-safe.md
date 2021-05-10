---
title: 需要將網域或電子郵件寄件者標示為安全嗎？
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
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286671"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a><span data-ttu-id="4717d-102">需要將網域或電子郵件寄件者標示為安全嗎？</span><span class="sxs-lookup"><span data-stu-id="4717d-102">Need to mark a domain or email sender safe?</span></span>

- <span data-ttu-id="4717d-103">我們 **不建議使用安全寄件者清單**，因為這會將組織暴露在垃圾郵件、網路釣魚詐騙和詐騙攻擊中。</span><span class="sxs-lookup"><span data-stu-id="4717d-103">Use of **safe sender lists is not recommended** since it opens up your organization to spam, phish, and spoofing attacks.</span></span>
- <span data-ttu-id="4717d-104">不過，如果有業務需求，我們 **建議** 使用 **[郵件流程規則](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。</span><span class="sxs-lookup"><span data-stu-id="4717d-104">However, if there is a business requirement, we **recommend** using **[Mail Flow Rules](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** for this.</span></span> <span data-ttu-id="4717d-105">我們的指導方針可確保寄件者驗證 (驗證送出網域未遭到假冒)。</span><span class="sxs-lookup"><span data-stu-id="4717d-105">Our guidance ensures sender authentication (verifies sending domain is not being spoofed).</span></span> <span data-ttu-id="4717d-106">**注意**：我們不建議使用安全的寄件者清單來管理誤判，因為垃圾郵件篩選的例外狀況可能會讓您的組織暴露在安全性攻擊中。</span><span class="sxs-lookup"><span data-stu-id="4717d-106">**Note**: We don't recommend managing false positives by using safe sender lists, because exceptions to spam filtering can open your organization to security attacks.</span></span> <span data-ttu-id="4717d-107">如果您的使用者收到錯誤標示為 [垃圾郵件] 的郵件，請 **[向 Microsoft 回報郵件和檔案](https://protection.office.com/reportsubmission)** (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="4717d-107">If your user(s) receive messages incorrectly marked as spam or junk email, please **[Report messages and files to Microsoft](https://protection.office.com/reportsubmission)**.</span></span>
- <span data-ttu-id="4717d-p102">**應避免** Outlook 中的安全寄件者、允許的寄件者清單或反垃圾郵件原則中的允許網域清單，因為寄件者人會繞過所有垃圾郵件、詐騙和網路魚防護以及寄件者驗證 (SPF、DKIM、DMARC)。此方法最適合用於單純的暫時測試。</span><span class="sxs-lookup"><span data-stu-id="4717d-p102">Safe Senders in Outlook, Allowed sender list, or allowed domain list in anti-spam policies **should be avoided** because senders bypass all spam, spoof, and phish protection, and sender authentication (SPF, DKIM, DMARC). This method is best used for temporary testing only.</span></span>
- <span data-ttu-id="4717d-110">驗證某封電子郵件是否略過反垃圾評估，可透過檢查 X-Forefront-Antispam-Report 郵件訊息標頭 (SFV:SFE, SFV:SKA, SFV:SKN)，請參閱 **[反垃圾郵件訊息標頭](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**。</span><span class="sxs-lookup"><span data-stu-id="4717d-110">The validation that a certain email bypassed Antispam evaluation can be done by checking “X-Forefront-Antispam-Report" message header (SFV:SFE, SFV:SKA, SFV:SKN), see **[Anti-spam message headers](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**.</span></span>
- <span data-ttu-id="4717d-111">因為 Microsoft 想要讓客戶保持 [預設安全性](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)，所以部分的租用戶覆寫並不適用於惡意程式碼或高信賴度網路釣魚。</span><span class="sxs-lookup"><span data-stu-id="4717d-111">Because Microsoft wants to keep our customers [secure by default](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions), some tenant overrides are not applied for malware and high confidence phishing.</span></span> <span data-ttu-id="4717d-112">這些覆寫包括: o   允許的寄件者清單或允許的網域清單 (反垃圾郵件原則) o   Outlook 安全寄件者 o   IP 允許清單 (連線篩選)</span><span class="sxs-lookup"><span data-stu-id="4717d-112">These overrides include: o   Allowed sender lists or allowed domain lists (anti-spam policies) o   Outlook Safe Senders o   IP Allow List (connection filtering)</span></span> 
- <span data-ttu-id="4717d-113">可允許高信賴度網路釣魚郵件略過篩選的唯一覆寫是 Exchange 郵件流程規則 (又稱為傳輸規則)。</span><span class="sxs-lookup"><span data-stu-id="4717d-113">The only override that allows high confidence phishing message to bypass filtering is Exchange mailflow rules (also known as transport rules).</span></span> <span data-ttu-id="4717d-114">若要使用郵件流程則略過篩選，請參閱 **[使用郵件流程規則在郵件中設定垃圾郵件信賴等級 (SCL)](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**。</span><span class="sxs-lookup"><span data-stu-id="4717d-114">To use mail flow rules to bypass filtering, see **[Use mail flow rules to set the spam confidence level (SCL) in messages](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**.</span></span>