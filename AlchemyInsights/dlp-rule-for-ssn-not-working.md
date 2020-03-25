---
title: SSN 無法運作的 DLP 規則
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
ms.openlocfilehash: 0b83a858975ffe1bb70f16a7452a13d57dff5340
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932512"
---
# <a name="dlp-issues-with-social-security-numbers"></a>使用社交安全性號碼的 DLP 問題

**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。 包括內容遷移、資料遺失防護（DLP）及備份解決方案。 在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。

為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。 您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。 不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。

**主旨 ssn 的 DLP 問題**

當您在 Office 365 中使用敏感資訊類型時，**資料遺失防護（DLP）** 未使用包含**社交安全性號碼（SSN）** 的內容時，是否發生問題？ 如果是的話，請確定您的內容包含 DLP 原則所要的內容所需的資訊。 
  
例如，對於設定置信級為85% 的 SSN 原則，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 位數（可能是格式化或未格式化的模式）

- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四種功能會在四種不同的模式中尋找主旨 ssn：

  - Func_ssn 會2011以主旨 ssn 的強格式格式化，並以短劃線或空格格式化（ddd-dd-dddd 或 ddd dd dddd）來尋找

  - Func_unformatted_ssn 會以預先2011的強格式格式化，以格式化為九個連續數位（ddddddddd）的主旨 ssn，來尋找

  - Func_randomized_formatted_ssn 會找到以短劃線或空格格式化的2011後主旨 ssn （ddd-dd-dddd 或 ddd dd dddd）

  - Func_randomized_unformatted_ssn 尋找未格式化為九個連續數位的2011後主旨 ssn （ddddddddd）

- **[Checksum：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** 否，沒有檢查

- **[定義：](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：

  - [函數 Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)找到符合模式的內容。

  - 會找到來自[Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn)的關鍵字。 關鍵字的範例包括：「*社會保險」、「社交安全性 #，Soc Sec，SSN* 。 例如，下列範例會觸發 DLP SSN 原則： **SSN： 489-36-8350**
  
如需針對您的內容偵測主旨 ssn 時所需的詳細資訊，請參閱本文的下列章節：[機密資訊類型針對主旨 ssn 的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)。
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊：[機密資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  