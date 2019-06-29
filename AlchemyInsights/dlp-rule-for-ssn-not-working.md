---
title: SSN 的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: fffd355279b064b31c0a8bf60518b15ee1ed1848
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389424"
---
# <a name="dlp-issues-with-social-security-numbers"></a>與社會保險號碼有關的 DLP 問題

您在 Office 365 中使用機密資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**社會保險號碼 (SSN)** 的內容時, 是否發生問題？ 如果是的話, 請確定您的內容包含 DLP 原則所要用的必要資訊。 
  
例如, 對於設定為信賴等級 85% 的 SSN 原則, 系統會評估下列專案, 並且必須偵測到要觸發的規則:
  
- **[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 位數, 可能是格式化或未格式化的模式

- **[模式:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四個函數在四種不同的模式中尋找主旨 ssn:

  - Func_ssn 找到主旨 ssn, 其格式為: 以虛線或空格格式化的預先2011強格式 (ddd-dd-dddd 或 ddd dd dddd)

  - Func_unformatted_ssn 找到主旨 ssn, 且具有非格式化為9個連續數位 (ddddddddd) 的2011之前強格式設定

  - Func_randomized_formatted_ssn 找到以虛線或空格格式化的 post 2011 主旨 ssn (ddd-dd-dddd 或 ddd dd dddd)

  - Func_randomized_unformatted_ssn 找到非格式化為九個連續數位的2011後主旨 ssn (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否, 沒有任何 Checksum

- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 85%:

  - [函數 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)找到符合模式的內容。

  - 找到[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)中的關鍵字。 關鍵字的範例包括:*社會保險、社會保險號碼、Soc Sec、SSN* 。 例如, 下列範例會觸發 DLP SSN 原則: **SSN: 489-36-8350**
  
如需偵測到內容主旨 ssn 所需的詳細資訊, 請參閱本文的下列章節:[敏感資訊類型對主旨 ssn 的搜尋](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  