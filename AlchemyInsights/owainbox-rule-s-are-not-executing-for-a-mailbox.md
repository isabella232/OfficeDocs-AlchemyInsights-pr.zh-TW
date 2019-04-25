---
title: 1332 OWA 位收件匣規則都不執行信箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1332
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: c0b221b5335254bd0f1eb4b258efa6946376ca12
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32372551"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>收件匣規則不會如預期般運作

確認下列設定：

- 郵件可以重新導向、 轉寄或回覆自動根據收件匣規則僅一次。 重新導向規則 （收件匣規則或郵件流程規則，也稱為傳輸規則） 可以將最大值為十個轉寄收件者新增至郵件。 如需詳細資訊，請參閱[日誌、 傳輸和收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。

- 收件匣規則不替代日誌記錄信箱上運作。 如需替代日誌記錄信箱的詳細資訊，請參閱 <<c0>替代日誌記錄信箱。

若要修正這些問題，請參閱 < <b0>KB 2829319</b0>。

如果不套用先前的問題，請向上呈報給 Microsoft 支援服務問題之前執行收件匣規則診斷報告：

1. 在網頁型 Outlook 中開啟信箱，然後按一下 [**設定** \> **選項** \> **組合管理電子郵件** \> **收件匣規則**。

2. 在頁面底部，按一下 [**您的規則如果無法使用 [按一下這裡以產生診斷報告**]。
