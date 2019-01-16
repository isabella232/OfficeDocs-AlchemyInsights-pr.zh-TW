---
title: SSN 無法正常運作的 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b92d122b774d97cd2e44cc0880dc5001065b57cc
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278395"
---
您已有**資料遺失防護 (DLP)** 無法正常運作的內容包含**社會安全號碼 (SSN)** 時使用 Office 365 中的敏感資訊類型的問題嗎？若是如此，請確定您的內容包含的 DLP 原則尋找的項目所需的資訊。 
  
例如 85%的信賴等級以設定 SSN 原則，下列會評估和必須偵測到的工作流程觸發此規則：
  
- **[格式：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 的數字，這可能是格式化或以未格式化的週期模式的 
    
- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四個不同的模式 SSNs 尋找四個函數： 
    
  - Func_ssn 都會尋找 SSNs 之前 2011年強式格式格式為虛線或空格 (ddd-dd-dddd OR ddd dd dddd)
    
  - Func_unformatted_ssn 都會尋找 SSNs 之前 2011年強式的格式以未格式化為九個連續的數字 (ddddddddd)
    
  - Func_randomized_formatted_ssn 都會以虛線或空格 (ddd-dd-dddd OR ddd dd dddd) 格式化的張貼 2011 SSNs
    
  - Func_randomized_unformatted_ssn 會尋找已格式化為九個連續的數字 (ddddddddd) 的文章 2011 SSNs
    
- **[總和檢查碼：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP 原則是 85%有信心它已偵測到這種類型的機密資訊時，300 個字元的距離： 
    
  - [函數 Func_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)會找出符合模式的內容。 
    
  - 從[Keyword_ssn](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)關鍵字是找到。關鍵字的範例包括：*社會安全、 社會安全 #、 Soc 秒、 SSN* 。例如，下列範例會觸發 DLP SSN 原則： **SSN: 489-36-8350**
    
什麼是 SSNs 偵測到的內容所需的詳細資訊，請參閱本文的下列章節：[什麼敏感資訊類型尋找 SSNs](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/en-us/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

