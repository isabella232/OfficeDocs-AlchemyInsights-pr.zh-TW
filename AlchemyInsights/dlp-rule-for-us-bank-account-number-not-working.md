---
title: 美國銀行帳戶號碼無法正常運作的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9fd5d4736c5209f85e235dc6a0846f65f1b5f624
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656990"
---
您已有**資料遺失防護 (DLP)** 無法正常運作的內容時使用 DLP 敏感資訊類型 O365 中包含**美國銀行帳戶號碼**的問題嗎？若是如此，請確定您的內容包含的 DLP 原則會尋找的項目時會評估當中所需的資訊。 
  
例如 85%的信賴等級以設定為**US 銀行帳戶號碼**原則，下列會評估和必須偵測到的工作流程觸發此規則： 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 位數 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8 17 連續的數字。 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP 原則就是有信心它已偵測到這種敏感資訊類型的 75 %if，300 個字元的距離： 
    
  - 規則運算式 Regex_usa_bank_account_number 會找出符合模式的內容
    
  - 找到來自於 Keyword_usa_Bank_Account 的關鍵字。
    
    例如，下列範例會觸發**美國銀行帳戶號碼**原則： 檢查帳戶 78344011 
    
什麼是**美國銀行帳戶號碼**來偵測的內容所需的詳細資訊，請參閱本文的下列章節：[什麼敏感資訊類型尋找美國銀行帳戶號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

