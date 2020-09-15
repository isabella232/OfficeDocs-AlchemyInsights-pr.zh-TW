---
title: 需要有關電子郵件傳送限制的協助嗎？
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
- "9002938"
- "5630"
ms.openlocfilehash: 66ff82afd7b44ef5fd4943bfc794c2fa35bbfa9e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702354"
---
# <a name="need-help-with-email-sending-limits"></a>需要有關電子郵件傳送限制的協助嗎？

以下是服務強制執行的**預設傳送限制**。 這些限制的詳細資訊記載在[這裡](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)。

- 若要防止傳送未經授權的大宗郵件，我們會為每位使用者套用**所有傳出和內部郵件的收件人比率限制**。 在所有 SKU 中，此限制為每天 **10,000 位收件者**。  客戶若需要傳送合法的大量商業電子郵件 (例如客戶電子報)，應使用專門提供這些服務的第三方供應商。
    - **注意**：達到收件人比率限制之後，就無法從信箱傳送郵件，除非收到郵件的收件者人數在過去 24 小時內減少到上限範圍內。 在那之前，使用者將無法傳送郵件。
- 所有 SKU 都會套用**每分鐘 30 封郵件**的郵件比率限制。 這個限制決定使用者在指定時間內可從 Exchange Online 帳戶傳送的郵件數量。
- 在所有 SKU 中，**[收件者]、[副本] 和 [密件副本]欄位允許的收件者數量上限**是 **1000 位收件人**。 若要自訂這個限制，請移至[這裡](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)。
