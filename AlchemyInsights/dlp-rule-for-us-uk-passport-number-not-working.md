---
title: 適用于美國/英國護照號碼的 DLP 規則未運作
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004937"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP-US/英國護照號碼的問題

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**美國/英國護照號碼的 DLP 問題**

當您在 O365 使用 DLP 敏感資訊類型時， **資料遺失防護 (dlp)** 無法處理包含 **美國/英國護照號碼** 的內容時，是否有問題？ 如果是的話，請確定您的內容中包含 DLP 原則在評估時所需的資訊。
  
例如，對於設定為信賴等級為75% 的 **美國/英國護照號碼** 原則，會評估下列各項，而且必須偵測到規則才能觸發
  
- **[格式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 九位數

- **[模式：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 九個連續數位

- **[Checksum：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** 否，沒有檢查

- **[定義：](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** 如果接近300個字元以內，則 DLP 原則偵測到此敏感資訊類型的置信量是75%：

  - 函數 Func_usa_uk_passport 找到符合模式的內容。

  - 會找到來自 Keyword_passport 的關鍵字。

    例如，下列範例會觸發 **美國/英國護照號碼** 原則：美國護照號碼123456789

如需針對您的內容偵測 US/英國護照號碼時所需的詳細資訊，請參閱本文的下列章節：[機密資訊類型針對美國/英國護照號碼所尋找的功能](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)。
  
使用不同的內建機密資訊類型，請參閱下列文章，以瞭解其他類型所需的資訊： [機密資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  