---
title: 建立使用者
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 742ff857141d08031302fdcff7e49b3eef90e0f7
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50718173"
---
# <a name="create-user"></a><span data-ttu-id="446a1-102">建立使用者</span><span class="sxs-lookup"><span data-stu-id="446a1-102">Create user</span></span>

<span data-ttu-id="446a1-103">**公告：**</span><span class="sxs-lookup"><span data-stu-id="446a1-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="446a1-104">[從 Google 開始，在2021年1月4日開始的 Web 視圖登入支援已過時](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 。</span><span class="sxs-lookup"><span data-stu-id="446a1-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="446a1-105">測試您的應用程式是否會受到 Google 對測試相容性 [的指導](https://go.microsoft.com/fwlink/?linkid=2157323) 所影響。</span><span class="sxs-lookup"><span data-stu-id="446a1-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="446a1-106">使用使用者 Google 帳戶登入時，請確定您使用系統 web 視圖或系統瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="446a1-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="446a1-107">如需詳細資訊，請參閱 [僅使用 Chrome 瀏覽器登入應用程式問題](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。</span><span class="sxs-lookup"><span data-stu-id="446a1-107">For more information, see [Issues signing in to application(s) using Chrome browser only](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="446a1-108">**我無法在我的 Azure Active Directory 中建立新使用者**</span><span class="sxs-lookup"><span data-stu-id="446a1-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="446a1-109">請確保您已獲授權建立新的標準使用者。</span><span class="sxs-lookup"><span data-stu-id="446a1-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="446a1-110">在 Azure Active Directory (AD) 中只有全域系統管理員或使用者系統管理員角色可以建立新的標準使用者。</span><span class="sxs-lookup"><span data-stu-id="446a1-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="446a1-111">如果您不是上述其中一種角色，請要求系統管理員將您新增為這些角色之一或為您建立新的使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="446a1-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="446a1-112">請確保使用者名稱所在的網域是在您的 Azure AD 得到驗證。</span><span class="sxs-lookup"><span data-stu-id="446a1-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="446a1-113">如果您的 Azure AD 中沒有任何已驗證的自訂網域名稱，您可以使用您的 Azure AD 初始網域，結尾是 \*. onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="446a1-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="446a1-114">請確保使用者名稱所在的網域並非是從內部部署 AD 同盟的 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="446a1-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="446a1-115">無法將使用者新增至具有從內部部屬同盟的網域名稱雲端中。</span><span class="sxs-lookup"><span data-stu-id="446a1-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="446a1-116">請確保其他使用者或聯絡人不具有您要指派給新使用者的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="446a1-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="446a1-117">使用者名稱在 Azure Active Directory 中必須是唯一的。</span><span class="sxs-lookup"><span data-stu-id="446a1-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="446a1-118">請參閱 Azure Active Directory 的 [Azure Active Directory 角色和系統管理員](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。</span><span class="sxs-lookup"><span data-stu-id="446a1-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="446a1-119">請參閱 Azure Active Directory 的 [網域名稱](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。</span><span class="sxs-lookup"><span data-stu-id="446a1-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="446a1-120">請檢視 [稽核記錄檔](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) 以查看更多關於最近建立或刪除的使用者的詳細資訊，例如誰執行該動作，以及何時執行。</span><span class="sxs-lookup"><span data-stu-id="446a1-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="446a1-121">如需新增使用者的詳細資訊，請參閱 [使用 azure 入口網站在 AZURE AD 中建立新的使用者](/azure/active-directory/active-directory-users-create-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="446a1-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="446a1-122">[AZURE AD 系統管理角色](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles)： Azure Active Directory 中的系統管理員角色許可權</span><span class="sxs-lookup"><span data-stu-id="446a1-122">[Azure AD administrative roles](https://docs.microsoft.com/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="446a1-123">您也可以 [使用 AZURE AD PowerShell 來建立新的使用者](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)。</span><span class="sxs-lookup"><span data-stu-id="446a1-123">You can also [use Azure AD PowerShell to create a new user](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
