---
title: 信箱接收限制強制執行
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/31/2021
ms.locfileid: "58829150"
---
# <a name="mailbox-receiving-limit-enforcement"></a>信箱接收限制強制執行

Microsoft 最近開始強制執行每個信箱每小時 3600 封郵件的閾值。 如需詳細資訊，請參閱 [Exchange Online 限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits)。 在一小時內接收超過 3600 封郵件的 Microsoft 365 信箱，會在接下來 60 分鐘進行節流。 

此外，還會套用可封鎖 Microsoft 365 信箱從特定寄件者所接收郵件的寄件者與收件者配對 (SRP) 限制。 如果單一寄件者每個滾動小時傳送超過總閾值的 33% 或 1200 封郵件給特定收件者，則會開始 SRP 限制，且信箱不再接受來自該寄件者的郵件。 請注意：

- 此限制會套用至來自其他租用戶、內部部署或網際網路寄件者的電子郵件。
- 將在接下來的 60 分鐘封鎖對信箱的電子郵件傳遞。 
- 這些信箱的寄件者會收到未傳遞報告 (5.2.121 或 5.2.122)，指出該信箱已超過傳遞閾值上限。 租用戶內部 (相同租用戶內的郵件) 則會繼續傳遞。
- 套用 SRP 限制時，接收端信箱會繼續接受來自其他寄件者的郵件。

系統管理員可以監視目前的信箱活動，方法是存取 Exchange 系統管理中心中名為「信箱超過接收限制」的新報告與深入解析。 只有當租用戶有違規的信箱時，才會顯示深入解析，同時報告一律會出現在儀表板中但為空白，除非租用戶有違規的信箱。

如需有關深入解析接收限制的詳細資訊，請參閱[新 EAC 中信箱超過接收限制深入解析](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)。

如需有關超過接收限制報告的詳細資訊，請參閱[新 EAC 中信箱超過接收限制報告](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)。