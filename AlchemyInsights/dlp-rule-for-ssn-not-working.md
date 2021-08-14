---
title: SSN 無法運作的 DLP 規則
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004973"
---
# <a name="dlp-issues-with-social-security-numbers"></a>使用社交安全性號碼的 DLP 問題

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**主旨 ssn 的 DLP 問題**

您的 **資料遺失防護是否有問題 (DLP)** 無法處理包含 **社會保險號碼的內容 (SSN)** 在 Microsoft 365 中使用敏感資訊類型時？ 如果是的話，請確定您的內容包含 DLP 原則所要的內容所需的資訊。 
  
例如，對於設定置信級為85% 的 SSN 原則，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 位數（可能是格式化或未格式化的模式）

- **[模式：](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** 四種功能會在四種不同的模式中尋找主旨 ssn：

  - Func_ssn 會找到主旨 ssn，其強格式為2011的強格式設定，格式為破折號或空格 (ddd-dd-dddd 或 ddd dd dddd) 

  - Func_unformatted_ssn 會以2011的預先設定格式將其強格式設定為九個連續位數 (ddddddddd 的主旨 ssn) 

  - Func_randomized_formatted_ssn 會找到以破折號或空格格式化的2011後主旨 ssn， (ddd-dd-dddd 或 ddd dd dddd) 

  - Func_randomized_unformatted_ssn (ddddddddd 中尋找未格式化為九個連續數位的2011後主旨 ssn) 

- **[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** 否，沒有檢查

- **[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：

  - [函數 Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80)找到符合模式的內容。

  - 會找到來自 [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) 的關鍵字。 關鍵字的範例包括：「  *社會保險」、「社交安全性 #，Soc Sec，SSN*  。 例如，下列範例會觸發 DLP SSN 原則： **SSN： 489-36-8350**
  
如需針對您的內容偵測主旨 ssn 時所需的詳細資訊，請參閱本文的下列章節：[機密資訊類型針對主旨 ssn 的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)。
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊： [機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  