---
title: API 許可權和同意
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932088"
---
# <a name="api-permissions-and-consent"></a>API 許可權和同意

與 Microsoft 身分識別平臺整合的應用程式遵循的授權模式，可讓使用者和系統管理員控制資料的存取方式。 已在 Microsoft 身分識別平臺端點上更新授權模型的實施。 它會變更應用程式必須與 Microsoft 身分識別平臺互動的方式。 [Microsoft 身分識別平臺端點中的許可權與同意](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)涵蓋此授權模型的基本概念，包括範圍、許可權和同意。

[Azure Active Directory (Azure AD) 同意架構](https://docs.microsoft.com/azure/active-directory/develop/consent-framework)，可讓您輕鬆開發多承租人 web 和原生用戶端應用程式。 這些應用程式允許從 Azure AD 租使用者登入，而不是應用程式註冊的使用者帳戶。 他們可能也需要存取 web APIs 例如 Microsoft Graph API (，以存取 Microsoft 365) 和其他 Microsoft 服務 ' APIs 中的 Azure AD、Intune 和服務，以及您自己的 web APIs。

