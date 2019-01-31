---
title: 美國的 DLP 規則 / 無法正常運作的英國護照號碼
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656414"
---
您有問題與無法正常運作的內容包含**資料遺失防護 (DLP)** **美國 / 英國護照號碼**時 O365 中使用 DLP 敏感資訊類型？若是如此，請確定您的內容包含的 DLP 原則會尋找的項目時會評估當中所需的資訊。 
  
例如，用於**美國 / 英國護照號碼**原則的 75%的信賴等級以設定下列會評估和必須以觸發規則偵測到 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 的數字 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續的數字 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 原則就是有信心它已偵測到這種敏感資訊類型的 75 %if，300 個字元的距離： 
    
  - 函數 Func_usa_uk_passport 找到符合模式的內容。
    
  - 找到來自於 Keyword_passport 的關鍵字。
    
    例如，下列範例會觸發的**美國 / 英國護照號碼**原則： US 護照號碼 123456789 
    
如需有關功能需要美國 / 英國護照號碼來偵測的內容，請參閱本文的下列章節：[什麼敏感資訊類型外觀如美國 / 英國護照號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
使用不同的內建敏感資訊類型，請參閱上功能所需的其他類型的資訊的下列文章：[尋找什麼敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

