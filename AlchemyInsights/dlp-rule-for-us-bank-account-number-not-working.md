---
title: 美國銀行帳戶號碼不使用 DLP 規則
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404260"
---
您遇到問題的**資料外洩防護 (DLP)** 無法運作時使用 O365 中的 DLP 敏感資訊類型，其中包含**美國銀行帳戶號碼**的內容？ 如果是的話，請確定您的內容包含的 DLP 原則會尋找的項目在評估時所需的資訊。 
  
例如，對於**美國銀行帳戶號碼**原則設定信賴等級的 85%，下列進行評估，並必須要觸發的規則偵測到： 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 個連續數字。 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP 原則是 75%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元： 
    
  - 規則運算式 Regex_usa_bank_account_number 找到符合模式的內容
    
  - 找不到來自 Keyword_usa_Bank_Account 的關鍵字。
    
    例如，下列範例會觸發**美國銀行帳戶號碼**原則： 檢查帳戶 78344011 
    
如需有關什麼是**美國銀行帳戶號碼**，才能偵測到您的內容所需的詳細資訊，請參閱這篇文章中的下列章節：[項目敏感資訊類型尋找美國銀行帳戶號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0>
  

