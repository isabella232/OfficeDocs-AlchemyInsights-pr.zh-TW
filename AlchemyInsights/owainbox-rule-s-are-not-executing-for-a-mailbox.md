---
title: 1332 OWA-收件匣規則未執行信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 7d1848830847fc6722da20e09a4875f49bf02bd3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35360908"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>收件匣規則無法如預期般運作

確認下列設定:

- 只能根據收件匣規則, 自動重新導向、轉寄或回復郵件一次。 重新導向規則 (收件匣規則或郵件流程規則, 也稱為傳輸規則) 最多可以新增十個轉寄收件者給郵件。 如需詳細資訊, 請參閱[日誌、傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。

- 收件匣規則無法在替代日誌記錄信箱上運作。 如需替代日誌記錄信箱的詳細資訊, 請參閱[替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。

若要修正這些問題, 請參閱[KB 2829319](https://support.microsoft.com/kb/2829319)。

如果未套用先前的問題, 請先執行收件匣規則診斷報告, 再將問題升級至 Microsoft 支援:

1. 在網頁版 Outlook 中開啟信箱, 然後按一下 [**設定** \> **選項** \> ] [**組織電子郵件** \> **收件匣規則**]。

2. 在頁面底部, 按一下 [**如果您的規則未運作], 請按一下此處產生診斷報告**。
