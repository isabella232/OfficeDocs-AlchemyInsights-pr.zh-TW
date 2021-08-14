---
title: 美國銀行帳戶號碼無法運作的 DLP 規則
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005009"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>美國銀行帳戶號碼的 DLP 問題

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**美國銀行帳戶號碼的 DLP 問題**

當您在 O365 使用 DLP 敏感資訊類型時， **資料遺失防護 (dlp)** 無法處理包含 **US 銀行帳戶號碼** 的內容時，是否有問題？ 如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。
  
例如，對於以信賴等級85% 設定的 **US 銀行帳戶號碼** 原則，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 位數

- **[Pattern：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 連續數位。

- **[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 否，沒有檢查

- **[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：

  - 正則運算式 Regex_usa_bank_account_number 找到符合模式的內容。

  - 會找到來自 Keyword_usa_Bank_Account 的關鍵字。

    例如，下列範例會觸發 **US 銀行帳戶號碼** 原則：檢查帳戶78344011

如需針對您的內容偵測到 **US 銀行帳戶** 所需的資訊，請參閱本文中的下列章節：[機密資訊類型針對 US 銀行帳戶所尋找的功能](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)。
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊： [機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  