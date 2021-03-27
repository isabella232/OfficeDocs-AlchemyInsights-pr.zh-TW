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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379793"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="d0c06-102">API 許可權和同意程式</span><span class="sxs-lookup"><span data-stu-id="d0c06-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="d0c06-103">若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。</span><span class="sxs-lookup"><span data-stu-id="d0c06-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="d0c06-104">[Microsoft graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference) 會列出與每個主要 Microsoft Graph APIs 集合相關聯的許可權。</span><span class="sxs-lookup"><span data-stu-id="d0c06-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="d0c06-105">此外，它也提供如何使用許可權的指導方針。</span><span class="sxs-lookup"><span data-stu-id="d0c06-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="d0c06-106">**設定或更新服務主體**</span><span class="sxs-lookup"><span data-stu-id="d0c06-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="d0c06-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) -這篇文章說明如何建立新的 serviceprincipal 物件。</span><span class="sxs-lookup"><span data-stu-id="d0c06-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="d0c06-108">[在入口網站中建立 AZURE AD app & 服務主體](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) -這篇文章說明如何建立新的 Azure Active Directory (azure ad) 應用程式和服務主體，可搭配以角色為基礎的存取控制使用。</span><span class="sxs-lookup"><span data-stu-id="d0c06-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="d0c06-109">[AZURE AD 中的應用程式 & 服務主體](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) -這篇文章說明 Azure Active Directory 中的應用程式註冊、應用程式物件和服務主體：其用途、使用方式，以及它們之間的相互關聯方式。</span><span class="sxs-lookup"><span data-stu-id="d0c06-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="d0c06-110">**新增或更新應用程式註冊，並提供系統管理員同意**</span><span class="sxs-lookup"><span data-stu-id="d0c06-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="d0c06-111">[建立應用程式註冊](https://docs.microsoft.com/graph/api/application-post-applications) -這篇文章說明如何建立新的 application 物件。</span><span class="sxs-lookup"><span data-stu-id="d0c06-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="d0c06-112">[更新應用程式註冊-API 許可權](https://docs.microsoft.com/graph/api/application-update) -這篇文章將告訴您如何更新 application 物件的屬性。</span><span class="sxs-lookup"><span data-stu-id="d0c06-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="d0c06-113">授與系統[管理員](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application)同意-若要讓系統管理員征與同意，我們需要管理員明確授與同意。</span><span class="sxs-lookup"><span data-stu-id="d0c06-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="d0c06-114">[RBAC (Beta) ](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) -role 管理容器，適用于 MICROSOFT 365 RBAC 提供者的統一角色定義和角色指派，可在單一角色指派中支援多個主體和多個範圍。</span><span class="sxs-lookup"><span data-stu-id="d0c06-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="d0c06-115">這不同于 *rbacApplication* 資源類型。</span><span class="sxs-lookup"><span data-stu-id="d0c06-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="d0c06-116">Microsoft Intune 是這類 RBAC 提供者的範例。</span><span class="sxs-lookup"><span data-stu-id="d0c06-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="d0c06-117">Intune 中的角色指派可以具有主體陣列及範圍群組的陣列。</span><span class="sxs-lookup"><span data-stu-id="d0c06-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="d0c06-118">**這是 Beta 版，這表示它仍在開發中，不建議用於生產環境。**</span><span class="sxs-lookup"><span data-stu-id="d0c06-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
