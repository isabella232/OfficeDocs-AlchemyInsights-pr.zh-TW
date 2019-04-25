---
title: DLP 規則的 SSN 沒有運作
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: d2d21fb5546d36990d69b76e3ceb72ce2edf3d80
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404408"
---
您遇到問題的**資料外洩防護 (DLP)** 無法運作時使用 Office 365 中的敏感資訊類型包含**社會安全號碼 (SSN)** 的內容？ 如果是的話，請確定您的內容包含用於 DLP 原則查詢所需的資訊。 
  
例如，對於 SSN 原則設定信賴等級的 85%，下列進行評估，並必須要觸發的規則偵測到：
  
- **[格式為：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 位數，可採用格式化或未格式化模式 
    
- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四個函數尋找 Ssn 四個不同的模式： 
    
  - Func_ssn 找到與預先 2011年強式的格式設定，以連字號或空格 (ddd ddd-dd-dddd 或 ddd dd dddd) 格式化 Ssn
    
  - Func_unformatted_ssn 找尋找 Ssn 具有預先 2011年強式的格式設定，會以未格式化為九個連續數字 (ddddddddd)
    
  - Func_randomized_formatted_ssn 找到以連字號或空格 (ddd ddd-dd-dddd 或 ddd dd dddd) 格式化的文章 2011 Ssn
    
  - Func_randomized_unformatted_ssn 找到 post 2011 Ssn 所格式化為九個連續數字 (ddddddddd)
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP 原則是 85%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元： 
    
  - [函數 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)找到符合模式的內容。 
    
  - 找不到來自[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)的關鍵字。 關鍵字的範例包括：*社會安全、 社會安全 #、 Soc Sec、 SSN* 。 例如，下列範例會觸發 DLP SSN 原則： **SSN: 489-36-8350**
    
如需有關為何需要 Ssn 偵測到您的內容的詳細資訊，請參閱這篇文章中的下列章節：[項目敏感資訊類型尋找 Ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0>
  

