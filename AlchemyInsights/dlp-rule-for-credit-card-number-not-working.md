---
title: 信用卡號無法正常運作的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657458"
---
您已有**資料遺失防護 (DLP)** 無法正常運作的內容時使用 DLP 敏感資訊類型 O365 中包含**信用卡號**的問題嗎？若是如此，請確定您的內容包含所需的資訊來觸發時會評估當中的 DLP 原則。例如**信用卡原則**設定的 85%的信賴等級，下列會評估和必須偵測到的工作流程觸發此規則： 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可格式化 (dddddddddddddddd) 和必須通過 Luhn 測試。 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 偵測從所有主要品牌全世界，包括因為撰寫、 Mastercard、 探索卡片、 JCB、 American Express、 gift 卡及大來卡卡很複雜且完善圖樣。 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是、 Luhn 總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP 原則是 85%有信心它已偵測到這種類型的機密資訊時，300 個字元的距離： 
    
  - 函數 Func_credit_card 找到符合模式的內容。
    
  - 下列其中一項為真： 
    
  - 找到來自於 Keyword_cc_verification 的關鍵字。
    
  - 找到從 Keyword_cc_name 關鍵字
    
  - 函數 Func_expiration_date 找到正確日期格式的日期。
    
  - 總和檢查碼會傳遞
    
    例如，在下列範例會觸發 DLP 信用卡號碼原則：
    
  - 因為撰寫： 4485 3647 3952 7352 
    
  - 到期： 2/2009
    
什麼是**信用卡號**來偵測的內容所需的詳細資訊，請參閱本文的下列章節：[什麼敏感資訊類型尋找信用卡 #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

