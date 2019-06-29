---
title: 信用卡號碼的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 5d3bdb3b074c485a2b19e934724ba6e74c84deae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389568"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>信用卡號碼的 DLP 問題

您在 O365 中使用 DLP 敏感資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**信用卡號碼**的內容時, 是否發生問題？ 如果是的話, 請確定您的內容包含在評估時觸發 DLP 原則所需的資訊。 例如, 對於設定為信賴等級 85% 的**信用卡原則**, 會評估下列專案, 並且必須偵測到要觸發的規則:
  
- **[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可以格式化或未格式化 (dddddddddddddddd), 且必須通過 Luhn 測試。

- **[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 一種非常複雜且健全的模式, 可偵測全球所有主要品牌的卡, 包括簽證、MasterCard、探索卡、JCB、北美版、禮品卡及 diner 卡。

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是, Luhn 校驗和

- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 85%:

  - 函數 Func_credit_card 找到符合模式的內容。

  - 下列其中一項為真:

  - 找到 Keyword_cc_verification 中的關鍵字。

  - 找到 Keyword_cc_name 中的關鍵字

  - 函數 Func_expiration_date 會找到正確日期格式的日期。

  - Checksum 會通過

    例如, 下列範例會觸發 DLP 信用卡號碼原則:

  - 簽證: 4485 3647 3952 7352
  
  - 過期: 2/2009

如需針對您的內容偵測**信用卡號碼**所需的詳細資訊, 請參閱本文的下列章節:[有關信用卡號碼的敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  