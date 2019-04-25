---
title: 無法使用的信用卡號碼的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e1d60c493a27efb7f724d57051e21fad5bd0242f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404470"
---
您遇到問題的**資料外洩防護 (DLP)** 無法運作時使用 O365 中的 DLP 敏感資訊類型，其中包含**信用卡號碼**的內容？ 如果是的話，請確定您的內容包含要觸發的所需的資訊的 DLP 原則評估時。 例如，對於**信用卡原則**設定信賴等級的 85%，下列會評估，並必須要觸發的規則偵測到： 
  
- **[格式為：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數，可格式化或未格式化 (dddddddddddddddd)，且必須通過 Luhn 測試。 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 偵測全球，包括 Visa、 Mastercard、 Discover Card、 JCB、 American Express、 禮品卡和大來卡所有主要品牌的非常複雜且健全的模式。 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP 原則是 85%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元： 
    
  - 函數 Func_credit_card 找到符合模式的內容。
    
  - 下列其中一項為真： 
    
  - 找不到來自 Keyword_cc_verification 的關鍵字。
    
  - 找到來自 Keyword_cc_name 的關鍵字
    
  - 函數 Func_expiration_date 找到正確日期格式的日期。
    
  - 總和檢查碼通過
    
    例如，下列範例會觸發 DLP 信用卡號碼原則：
    
  - Visa: 4485 3647 3952 7352 
    
  - 到期： 2/2009
    
如需有關為何需要**Credit Card Number** ，偵測到您的內容的詳細資訊，請參閱這篇文章中的下列章節：[項目敏感資訊類型尋找信用卡 #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0>
  

