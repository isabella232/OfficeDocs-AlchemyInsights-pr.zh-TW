---
title: 適用于 US 銀行帳戶號碼的 DLP 規則無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 83050b05cffacd3e81d34f05383c213eb0042fae
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389460"
---
當您在 O365 中使用 DLP 敏感資訊類型時, 遇到**資料遺失防護 (DLP)** 無法使用包含**US 銀行帳戶號碼**的內容時, 是否發生問題？ 若是如此, 請確定您的內容包含在評估時, DLP 原則所尋找的必要資訊。
  
例如, 對於以信賴等級 85% 設定的**US 銀行帳戶號碼**原則, 會評估下列專案, 並且必須偵測到要觸發的規則:
  
- **[格式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數

- **[模式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 連續數位。

- **[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否, 沒有任何 Checksum

- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果接近300個字元以內, 則 DLP 原則偵測到此敏感資訊類型的置信度 75%:

  - 正則運算式 Regex_usa_bank_account_number 找到符合模式的內容

  - 找到 Keyword_usa_Bank_Account 中的關鍵字。

    例如, 下列範例會觸發**美國銀行帳戶號碼**原則: 檢查帳戶78344011

如需針對您的內容偵測到**美國銀行帳戶**所需的詳細資訊, 請參閱本文中的下列章節:[敏感資訊類型對美國銀行帳戶號碼的檢查](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
使用不同的內建機密資訊類型, 請參閱下列文章, 以瞭解其他類型所需的資訊:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  