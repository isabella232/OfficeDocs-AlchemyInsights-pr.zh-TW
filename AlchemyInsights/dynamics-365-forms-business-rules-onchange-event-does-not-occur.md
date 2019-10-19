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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36529010"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="aeb69-102">如果欄位以程式設計方式變更不會發生 OnChange 事件</span><span class="sxs-lookup"><span data-stu-id="aeb69-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="aeb69-103">如果使用以程式設計方式變更欄位的*OnChange*事件不會發生*屬性。*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue)方法。</span><span class="sxs-lookup"><span data-stu-id="aeb69-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="aeb69-104">如果您想要執行您在設定值，您必須使用之後的*OnChange*事件的事件處理常式*formContext.data.entity 屬性。* 在您的程式碼中的[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange)方法。</span><span class="sxs-lookup"><span data-stu-id="aeb69-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute.*[fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
