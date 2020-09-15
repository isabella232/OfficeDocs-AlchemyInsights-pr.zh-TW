---
title: 信用卡號碼的 DLP 規則無法運作
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679432"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>使用信用卡問題的 DLP 問題

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**使用信用卡問題的 DLP 問題**

當您在 O365 使用 DLP 敏感資訊類型時， **資料遺失防護 (dlp) ** 無法處理包含 **信用卡號碼** 的內容時，是否有問題？ 如果是的話，請確定您的內容包含必要資訊，以便在評估時觸發 DLP 原則。 例如，對於設定為信賴等級85% 的 **信用卡原則** ，會評估下列專案，而且必須偵測到要觸發的規則：
  
- **[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 位數，可格式化或未格式化 (dddddddddddddddd) ，且必須通過 Luhn 測試。

- **[模式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** 非常複雜且健全的模式，可偵測全球所有主要品牌的卡，包括簽證、MasterCard、探索卡、JCB、美洲 Express、禮品卡和 diner 卡。

- **[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** 是，Luhn 檢查碼

- **[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是85%：

  - 函數 Func_credit_card 找到符合模式的內容。

  - 下列其中一項為真：

  - 會找到來自 Keyword_cc_verification 的關鍵字。

  - 找到來自 Keyword_cc_name 的關鍵字

  - 函數 Func_expiration_date 會找到正確日期格式的日期。

  - Checksum 會通過

    例如，下列範例會觸發 DLP 信用卡號碼原則：

  - 簽證： 4485 3647 3952 7352
  
  - 到期：2/2009

如需針對您的內容偵測 **信用卡號碼** 所需的詳細資訊，請參閱本文中的下一節： [機密資訊類型針對信用卡號碼的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊： [機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  