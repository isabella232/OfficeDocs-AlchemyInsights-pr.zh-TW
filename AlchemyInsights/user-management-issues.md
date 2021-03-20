---
title: 使用者管理問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897774"
---
# <a name="user-management-issues"></a><span data-ttu-id="bcb5c-102">使用者管理問題</span><span class="sxs-lookup"><span data-stu-id="bcb5c-102">User management issues</span></span>

<span data-ttu-id="bcb5c-103">**如果我停用屬性 '需要使用者指派' (將此屬性設定為 No)，目前已指派給應用程式的使用者會發生什麼情況？**</span><span class="sxs-lookup"><span data-stu-id="bcb5c-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="bcb5c-104">停用 **[需要使用者指派]** 不會影響目前已指派的使用者。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="bcb5c-105">停用此屬性只會允許所有使用者存取應用程式。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="bcb5c-106">所有列出的使用者，以及已指派給應用程式中群組的使用者仍然有效。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="bcb5c-107">若要將您的應用程式限制為特定一組使用者，請參閱 - [Azure AD 應用程式限制一組使用者 - Microsoft 身分識別平台 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="bcb5c-108">若要指派使用者和群組至 Azure Active Directory (Azure AD) 中的企業應用程式 (從 Azure 入口網站內或使用 PowerShell)，請參閱[在 Azure Active Directory 中管理應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="bcb5c-109">若要委派應用程式建立和管理權限，請參閱[委派應用程式管理系統管理員權限 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="bcb5c-110">**向使用者隱藏特定企業應用程式** - 使用下列步驟，從 **MyApps** 面板中隱藏所有 Microsoft 365 應用程式。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="bcb5c-111">應用程式仍然顯示在 Office 365 入口網站中。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="bcb5c-112">以您目錄的全域管理員身分登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="bcb5c-113">選取 **[Azure Active Directory]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="bcb5c-114">選取 **[使用者]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="bcb5c-115">選取 **[使用者設定]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="bcb5c-116">在 **[企業應用程式]** 下，按一下 **[管理終端使用者如何啟動和檢視其應用程式]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="bcb5c-117">針對 **[使用者只能在 Office 365 入口網站中查看 Office 365 應用程式]**，請按一下 **[是]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="bcb5c-118">按一下 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="bcb5c-119">有關詳細資料，請參閱 [在 Azure AD 中隱藏使用者的企業應用程式之體驗 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.) (部分機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="bcb5c-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="bcb5c-120">如果您提供軟體即服務 (SaaS) 應用程式給許多組織，您可以將應用程式設定為接受來自任何 Azure Active Directory (Azure AD) 租用戶的登入。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="bcb5c-121">此設定稱為「將您的應用程式設為多租用戶」。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="bcb5c-122">任何 Azure AD 租用戶中的使用者，在同意將他們的帳戶用於您的應用程式之後，就可以登入您的應用程式。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="bcb5c-123">有關詳細資訊，請參閱 [建立登入 Azure AD 使用者的應用程式 - Microsoft 身分識別平台 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="bcb5c-124">**終端用者被指派至應用程式後，如何存取應用程式？**</span><span class="sxs-lookup"><span data-stu-id="bcb5c-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="bcb5c-125">企業應用程式刀鋒視窗中的每個應用程式都有供使用者存取的連結。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="bcb5c-126">使用者也可以透過 **MyApps** 入口網站輕鬆存取應用程式。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="bcb5c-127">**想知道使用者所使用的應用程式和應用程式類型嗎？**</span><span class="sxs-lookup"><span data-stu-id="bcb5c-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="bcb5c-128">您可以從 **portal.azure.com > Azure Active Directory> 登入> 下載報告** 下載最近 30 天的登入報告。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="bcb5c-129">了解如何[將整個租用戶系統管理員同意授與給應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) (部分機器翻譯) 和[設定使用者同意應用程式的方式](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="bcb5c-130">了解[同意的運作方式](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) (部分機器翻譯) 和[管理應用程式的同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="bcb5c-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>


