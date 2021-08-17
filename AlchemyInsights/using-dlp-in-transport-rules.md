---
title: 在傳輸規則中使用 DLP
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: ebc0fb718eb0572e849c5d780977deaee480a00c2825c18a12e4d2212342f17a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54084085"
---
# <a name="using-dlp-in-transport-rules"></a>在傳輸規則中使用 DLP

若要將資料遺失防護 (DLP) 整合至現有傳輸，請使用 [傳輸規則] 設定中的 **如果郵件包含...機密資訊** 條件。

**如需詳細資訊，請參閱：**

- 傳輸規則中整合的 DLP 機密資訊類型：[整合機密資訊規則](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules)。

您也可以使用規則上的測試模式，利用原則測試或不利用原則測試來測試規則。  建立規則後、測試之前，請先等候 30 分鐘。

- 請參閱[測試郵件流程/傳輸規則](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)

**注意**：如果您嘗試使用 EAC 中的傳輸規則來實作新的 DLP 原則，請改用 [安全性與合規性中心中的 DLP 原則](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide)。
