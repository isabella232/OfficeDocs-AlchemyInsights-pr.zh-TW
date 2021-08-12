---
title: API 許可權和同意程式
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932052"
---
# <a name="api-permissions-and-consent-process"></a>API 許可權和同意程式

若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。 [microsoft Graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference)會列出與每一組主要 Microsoft Graph APIs 相關聯的許可權。 此外，它也提供如何使用許可權的指導方針。

**設定或更新服務主體**

- [Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) -這篇文章說明如何建立新的 serviceprincipal 物件。
- [在入口網站中建立 Azure AD app & 服務主體](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)-這篇文章說明如何建立新的 Azure Active Directory (Azure ad) 應用程式和服務主體，可搭配以角色為基礎的存取控制。
- [Azure AD 中的應用程式 & 服務主體](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)-這篇文章說明 Azure Active Directory 中的應用程式註冊、應用程式物件和服務主體：定義及其使用方式及其相互關聯的方式。

**新增或更新應用程式註冊，並提供系統管理員同意**

- [建立應用程式註冊](https://docs.microsoft.com/graph/api/application-post-applications) -這篇文章說明如何建立新的 application 物件。
- [更新應用程式註冊-API 許可權](https://docs.microsoft.com/graph/api/application-update) -這篇文章將告訴您如何更新 application 物件的屬性。
- 授與系統[管理員](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application)同意-若要讓系統管理員征與同意，我們需要管理員明確授與同意。
- [rbac (Beta) ](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) -role 管理容器，可在單一角色指派中支援多個主體和多個範圍的 Microsoft 365 RBAC 提供者使用統一角色定義和角色指派。 這不同于 *rbacApplication* 資源類型。 Microsoft Intune 為這類 RBAC 提供者的範例。 Intune 中的角色指派可以具有主體陣列及範圍群組的陣列。 **這是 Beta 版，這表示它仍在開發中，不建議用於生產環境。**
