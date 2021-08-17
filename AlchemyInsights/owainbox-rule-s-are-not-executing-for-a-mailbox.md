---
title: 1332 OWA-收件匣規則 (s) 不會執行信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040893"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>收件匣規則未如期運作

在 Outlook 網頁版中驗證下列設定：

- 郵件只能根據收件匣規則，自動重新導向、轉寄或回復一次。 重新導向規則 (收件匣規則或郵件流程規則（也稱為傳輸規則) ）最多可將十個轉寄收件者新增至郵件。 如需詳細資訊，請參閱 [日誌、傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。

- 收件匣規則不適用於替代日誌記錄信箱。 如需替代日誌記錄信箱的詳細資訊，請參閱 [替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。

若要修正這些問題，請參閱 [KB 2829319](https://support.microsoft.com/kb/2829319)。

若未套用上述問題，請先執行收件匣規則診斷報告，再將問題提升至 Microsoft 支援：

1. 在 Outlook 網頁版中開啟信箱，然後按一下 <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **設定**  > **全部查看 Outlook 設定**  > **郵件**  > **規則**。

2. 在頁面底部，按一下 [ **如果規則未正常運作]，請按一下這裡以產生診斷報告**。
