---
title: 需要將網域或電子郵件寄件者標示為安全嗎？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803236"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>需要將網域或電子郵件寄件者標示為安全嗎？

- 我們**不建議使用安全寄件者清單**，因為這會將組織暴露在垃圾郵件、網路釣魚詐騙和詐騙攻擊中。
- 不過，如果有業務需求，我們**建議**使用**[郵件流程規則](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)**。 我們的指導方針可確保寄件者驗證 (驗證送出網域未遭到假冒)。 **注意**：我們不建議使用安全的寄件者清單來管理誤判，因為垃圾郵件篩選的例外狀況可能會讓您的組織暴露在安全性攻擊中。 如果您的使用者收到錯誤標示為 [垃圾郵件] 的郵件，請**[向 Microsoft 回報郵件和檔案](https://protection.office.com/reportsubmission)** (部分機器翻譯)。
- 應避免**** Outlook 中的安全寄件者、允許的寄件者清單或反垃圾郵件原則中的允許網域清單，因為寄件者人會繞過所有垃圾郵件、詐騙和網路魚防護以及寄件者驗證 (SPF、DKIM、DMARC)。 這個方法最適合用來進行暫時測試。
