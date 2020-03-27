---
title: 美國銀行帳戶號碼無法運作的 DLP 規則
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
ms.openlocfilehash: bb7d8ca91af73fa4ebed5992ec848128beb18830
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977153"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>美國銀行帳戶號碼的 DLP 問題

**重要**事項：在這些空前的時間內，我們採取步驟來確保 SharePoint 線上和 OneDrive 服務保持高可用性–請流覽[SharePoint 線上暫存功能](https://aka.ms/ODSPAdjustments)，以取得詳細資訊。

**美國銀行帳戶號碼的 DLP 問題**

當您在 O365 中使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 的內容無法使用包含**US 銀行帳號**的內容時，是否發生問題？ 如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。
  
例如，對於以信賴等級85% 設定的**US 銀行帳戶號碼**原則，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 位數

- **[Pattern：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 連續數位。

- **[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** 否，沒有檢查

- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：

  - 正則運算式 Regex_usa_bank_account_number 找到符合模式的內容。

  - 會找到來自 Keyword_usa_Bank_Account 的關鍵字。

    例如，下列範例會觸發**US 銀行帳戶號碼**原則：檢查帳戶78344011

如需針對您的內容偵測到**US 銀行帳戶**所需的資訊，請參閱本文中的下列章節：[機密資訊類型針對 US 銀行帳戶所尋找的功能](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)。
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  