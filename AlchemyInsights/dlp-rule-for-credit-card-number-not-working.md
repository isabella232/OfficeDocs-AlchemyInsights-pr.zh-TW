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
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932434"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>使用信用卡問題的 DLP 問題

**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。 包括內容遷移、資料遺失防護（DLP）及備份解決方案。 在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。

為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。 您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。 不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。

**使用信用卡問題的 DLP 問題**

當您在 O365 使用 DLP 敏感資訊類型時，**資料遺失防護（DLP）** 未針對包含**信用卡號碼**的內容運作時，是否發生問題？ 如果是的話，請確定您的內容包含必要資訊，以便在評估時觸發 DLP 原則。 例如，對於設定為信賴等級85% 的**信用卡原則**，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 位數可格式化或未格式化（dddddddddddddddd），且必須通過 Luhn 測試。

- **[模式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** 非常複雜且健全的模式，可偵測全球所有主要品牌的卡，包括簽證、MasterCard、探索卡、JCB、美洲 Express、禮品卡和 diner 卡。

- **[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** 是，Luhn 檢查碼

- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：

  - 函數 Func_credit_card 找到符合模式的內容。

  - 下列其中一項為真：

  - 會找到來自 Keyword_cc_verification 的關鍵字。

  - 找到來自 Keyword_cc_name 的關鍵字

  - 函數 Func_expiration_date 會找到正確日期格式的日期。

  - Checksum 會通過

    例如，下列範例會觸發 DLP 信用卡號碼原則：

  - 簽證： 4485 3647 3952 7352
  
  - 到期：2/2009

如需針對您的內容偵測**信用卡號碼**所需的詳細資訊，請參閱本文中的下一節：[機密資訊類型針對信用卡號碼的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  