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
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326068"
---
# <a name="outbound-relay-pool"></a>輸出轉送集區

Microsoft 正在對設定進行一些變更，以透過 Microsoft 365 轉送或轉寄電子郵件。 特定案例中的郵件會透過 Microsoft 365 使用特殊轉送集區轉寄或轉送。 使用轉送集區傳送的郵件會在收件者的 [垃圾郵件] 資料夾中結束。 如需詳細資訊，請參閱[輸出傳遞](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)集區

若要避免使用轉送集區的情況，請確定轉寄/轉送郵件符合下列其中一個條件：

- 輸出寄件者是租使用者的網域。
- 當郵件 Microsoft 365 時，寄件者原則框架 (SPF) 傳送。
- 當郵件到達 Microsoft 365 時，DomainKeys 身分識別的郵件 (DKIM) 在 P2 寄件者網域上傳遞。
 
符合上述準則的郵件不會透過轉送集區中繼。

如果您網域的 MX 記錄指向協力廠商或內部部署伺服器，請使用增強型篩選，以確定輸入電子郵件的 SPF 驗證是否正確，以及避免透過轉送集區傳送電子郵件。

**如何判斷我們是否受到轉送集區的影響？**

如果轉寄或轉送的電子郵件使用上述其中一個條件，則郵件將不會透過轉送集區中繼。 不過，如果透過轉送集區傳送郵件，則輸出伺服器 IP 是在 40.95.0.0/16 範圍內，而外寄伺服器名稱則包含 **rly** 的名稱。

