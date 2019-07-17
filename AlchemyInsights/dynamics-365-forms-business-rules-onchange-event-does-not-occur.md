---
title: Dynamics 365 形成商務規則的商務規則未引發表單
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/16/2019
ms.locfileid: "35747083"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>如果欄位以程式設計方式變更不會發生 OnChange 事件

如果使用以程式設計方式變更欄位的*OnChange*事件不會發生*屬性。*[setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)方法。 如果您想要執行您在設定值，您必須使用之後的*OnChange*事件的事件處理常式*formContext.data.entity 屬性。* 在您的程式碼中的[fireOnchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)方法。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
