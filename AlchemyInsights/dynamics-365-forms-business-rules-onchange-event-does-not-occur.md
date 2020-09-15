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
ms.openlocfilehash: 7422b67973f93ce10c1639209cc50206a1016c10
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711482"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="f7927-102">如果此欄位是以程式設計方式變更，則不會發生 OnChange 事件。</span><span class="sxs-lookup"><span data-stu-id="f7927-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="f7927-103">如果欄位是以程式設計方式使用屬性變更，則不會發生 *OnChange* 事件 *。*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) 方法。</span><span class="sxs-lookup"><span data-stu-id="f7927-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="f7927-104">如果您要在設定值之後執行 *OnChange* 事件的事件處理常式，則必須在您的程式碼中使用 *formCoNtext 屬性* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) 方法。</span><span class="sxs-lookup"><span data-stu-id="f7927-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
