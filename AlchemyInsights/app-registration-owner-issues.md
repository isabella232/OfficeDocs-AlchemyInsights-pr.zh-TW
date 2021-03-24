---
title: 應用程式註冊擁有人問題
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123114"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="6064c-102">應用程式註冊擁有人問題</span><span class="sxs-lookup"><span data-stu-id="6064c-102">App Registration Owner issues</span></span>

<span data-ttu-id="6064c-103">以下是可將主體新增為應用程式註冊負責人的可用方法：</span><span class="sxs-lookup"><span data-stu-id="6064c-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="6064c-104">使用 Azure AD PowerShell 模組-</span><span class="sxs-lookup"><span data-stu-id="6064c-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="6064c-105">參考： [載入 AzureADApplicationOwner (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="6064c-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="6064c-106">使用 Azure CLI- `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="6064c-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="6064c-107">參照： [az ad 應用程式擁有](https://docs.microsoft.com/cli/azure/ad/app/owner)者</span><span class="sxs-lookup"><span data-stu-id="6064c-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="6064c-108">使用 MS Graph-</span><span class="sxs-lookup"><span data-stu-id="6064c-108">Using MS Graph -</span></span>

    <span data-ttu-id="6064c-109">參考：[新增擁有者-Microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-post-owners)版</span><span class="sxs-lookup"><span data-stu-id="6064c-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="6064c-110">使用 Azure AD 入口網站-流覽至 [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > 應用程式註冊 > 選取應用程式 > 擁有者 > 新增擁有者</span><span class="sxs-lookup"><span data-stu-id="6064c-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="6064c-111">**即使您是該應用程式的擁有者，也無法在應用程式註冊 blade 上查看您的應用程式？**</span><span class="sxs-lookup"><span data-stu-id="6064c-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="6064c-112">應用程式的擁有者不是系統管理角色。</span><span class="sxs-lookup"><span data-stu-id="6064c-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="6064c-113">如果已啟用設定 [ [限制存取 AZURE AD 管理入口網站](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) ]，則只有系統管理員可以在應用程式註冊入口網站上查看應用程式。</span><span class="sxs-lookup"><span data-stu-id="6064c-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="6064c-114">若要讓擁有者能夠查看應用程式，請停用此設定 (將此設定設為 [) 否]，或將系統管理員角色指派給擁有者，只指定特定的應用程式。</span><span class="sxs-lookup"><span data-stu-id="6064c-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="6064c-115">不過，您必須使用 Azure AD Premium P2 授權，並啟用許可權身分 [識別管理](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)。</span><span class="sxs-lookup"><span data-stu-id="6064c-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
