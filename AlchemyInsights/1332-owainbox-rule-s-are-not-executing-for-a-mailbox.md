---
title: 1332 OWA 位收件匣規則未執行信箱
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f090d0a9d84bc6a4d1a1f4c0af55102d4b0ddfbe
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279166"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>收件匣規則不會在如預期般運作

確認下列設定：
  
- 訊息可以重新導向、 轉寄或回覆自動根據收件匣規則只有一次。正在重新導向規則 （收件匣規則或郵件流程規則，也稱為傳輸規則） 可以新增十轉寄的收件者的最大值的郵件。如需詳細資訊，請參閱[日誌、 傳輸及收件匣規則限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)。
    
- 替代日誌記錄信箱不處理收件匣規則。如需備用日誌記錄信箱的詳細資訊，請參閱[替代日誌記錄信箱](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox)。
    
若要修正這些問題，請參閱[KB 2829319](https://support.microsoft.com/kb/2829319)。
  
如果未套用先前問題呈報給 Microsoft 支援問題之前執行收件匣規則診斷報告：
  
1. 在 web 上的 Outlook 開啟信箱並按一下 [**設定** \> **選項** \> **組織電子郵件** \> **收件匣規則**。
    
2. 在頁面的底端，按一下 [**如果規則無法使用 [按一下此處產生的診斷報告**。
    

