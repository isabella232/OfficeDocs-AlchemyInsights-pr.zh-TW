---
title: 資源或服務主體的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2021
ms.locfileid: "50716122"
---
# <a name="issues-with-a-resource-or-service-principal"></a><span data-ttu-id="16049-102">資源或服務主體的問題</span><span class="sxs-lookup"><span data-stu-id="16049-102">Issues with a Resource or Service Principal</span></span>

1. <span data-ttu-id="16049-103">如果您剛剛開始， [Azure Active directory 中的應用程式和服務主體物件](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) 會描述 Azure active directory 中的應用程式註冊、應用程式物件和服務主體：其用途、使用方式，以及它們之間的相互關聯方式。</span><span class="sxs-lookup"><span data-stu-id="16049-103">If you are just getting started, [Application and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span> <span data-ttu-id="16049-104">同時也會呈現多承租人範例案例，以說明應用程式的應用程式物件與對應服務主體物件之間的關係。</span><span class="sxs-lookup"><span data-stu-id="16049-104">A multi-tenant example scenario is also presented to illustrate the relationship between an application's application object and corresponding service principal objects.</span></span>
2. <span data-ttu-id="16049-105">您可以 [在 Azure Active Directory 中讀取應用程式和服務主體物件](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)，深入瞭解應用程式和服務主體之間的關係。</span><span class="sxs-lookup"><span data-stu-id="16049-105">You can learn more about the relationship between applications and service principals by reading [applications and service principal objects in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).</span></span>
3. <span data-ttu-id="16049-106">[操作方法：使用入口網站建立可以存取資源的 AZURE ad 應用程式和服務主體](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) 顯示如何建立新的 Azure Active Directory (azure ad) 應用程式和服務主體，可搭配角色的存取控制使用。</span><span class="sxs-lookup"><span data-stu-id="16049-106">[How to: Use the portal to create an Azure AD application and service principal that can access resources](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
4. <span data-ttu-id="16049-107">使用 [服務主體 API](https://docs.microsoft.com/graph/api/resources/serviceprincipal)，您可以以程式設計方式管理應用程式的實例，並控制應用程式在您的租使用者中可以執行的作業。</span><span class="sxs-lookup"><span data-stu-id="16049-107">With the [service principal API](https://docs.microsoft.com/graph/api/resources/serviceprincipal), you can programmatically manage instances of applications and control what an application can do within your tenant.</span></span>
5. <span data-ttu-id="16049-108">[servicePrincipal 資源類型](https://docs.microsoft.com/graph/api/resources/serviceprincipal) 會列出 servicePrincipal 資源類型的所有屬性和方法。</span><span class="sxs-lookup"><span data-stu-id="16049-108">[servicePrincipal resource type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) lists all properties and methods for the servicePrincipal resource type.</span></span>
6. <span data-ttu-id="16049-109">[AZURE Ad graph 和 Microsoft graph 之間的資源類型差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) 會強調 Azure ad Graph 和 microsoft graph 資源之間的差異。</span><span class="sxs-lookup"><span data-stu-id="16049-109">[Resource type differences between Azure AD Graph and Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) highlights differences between Azure AD Graph and Microsoft Graph resources.</span></span> <span data-ttu-id="16049-110">它會顯示具有不同名稱或無法使用的資源。它也會強調 Microsoft Graph Beta 版中可用的資源，但不是在第1.0 版中。</span><span class="sxs-lookup"><span data-stu-id="16049-110">It shows resources that have different names or are not available; it also highlights resources available in the beta version of Microsoft Graph but not in the v1.0 version.</span></span>

<span data-ttu-id="16049-111">**來賓使用者的問題**</span><span class="sxs-lookup"><span data-stu-id="16049-111">**Issues with Guest Users**</span></span>

- <span data-ttu-id="16049-112">[快速入門：將來賓使用者新增至 azure 入口網站中的目錄](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) 顯示如何透過 azure 入口網站將新的來賓使用者新增至 Azure AD 目錄、傳送邀請，以及查看來賓使用者的邀請函兌換處理常式的外觀。</span><span class="sxs-lookup"><span data-stu-id="16049-112">[Quickstart: Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) shows you how to add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
- <span data-ttu-id="16049-113">[教程：在 Azure Active DIRECTORY B2C 中建立使用者資料流程](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) 您可以透過使用 Azure 入口網站來建立某些建議的使用者流程。</span><span class="sxs-lookup"><span data-stu-id="16049-113">[Tutorial: Create user flows in Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) shows you how to create some recommended user flows by using the Azure portal.</span></span> <span data-ttu-id="16049-114">如果您正在尋找如何在應用程式中設定資源擁有者密碼認證 (ROPC) 流程的相關資訊，請參閱在 Azure AD B2C 中設定資源擁有者密碼認證流程。</span><span class="sxs-lookup"><span data-stu-id="16049-114">If you are looking for information about how to set up a resource owner password credentials (ROPC) flow in your application, see Configure the resource owner password credentials flow in Azure AD B2C.</span></span>
