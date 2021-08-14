---
title: Dynamics 365 Forms Business Rules-表單未引發商務規則
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 8425918950e1ef6c44f2866e6fa8987fe165536ae21e08ea6a1da880f761d512
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53947290"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>如果此欄位是以程式設計方式變更，則不會發生 OnChange 事件。

如果欄位是以程式設計方式使用屬性變更，則不會發生 *OnChange* 事件 *。*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) 方法。 如果您要在設定值之後執行 *OnChange* 事件的事件處理常式，則必須在您的程式碼中使用 *formCoNtext 屬性* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) 方法。

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
