---
title: DLP 規則如美國 / 不使用 UK 護照號碼
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: bb80ef07364a575f6032bb105cff83cd8f95bd63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404372"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>問題 DLP-美國 / 英國護照號碼

您有問題**的資料外洩防護 (DLP)** 無法使用的內容包含**美國 / 英國護照號碼**時使用 O365 中的 DLP 敏感資訊類型？ 如果是的話，請確定您的內容包含的 DLP 原則會尋找的項目在評估時所需的資訊。 
  
例如，針對**美國 / 英國護照號碼**75%的信賴等級所設定的原則，下列會評估和必須偵測到要觸發的規則 
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 九位數 
    
- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 九個連續數字 
    
- **[總和檢查碼：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有任何總和檢查碼 
    
- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP 原則是 75%以內，已偵測到此敏感資訊類型的如果鄰近性是 300 個字元： 
    
  - 函數 Func_usa_uk_passport 找到符合模式的內容。
    
  - 找不到來自 Keyword_passport 的關鍵字。
    
    例如，下列範例會觸發的**美國 / 英國護照號碼**原則： 美國護照號碼 123456789 
    
如需有關為何需要美國 / 英國護照號碼，才能偵測到您的內容，請參閱本文中的下列區段：[美國的項目敏感資訊類型尋找 / 英國護照號碼](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
使用不同的內建敏感資訊類型，請參閱 < 上為何需要其他類型的資訊的下列文章：<b0>項目敏感資訊類型在找</b0>
  

