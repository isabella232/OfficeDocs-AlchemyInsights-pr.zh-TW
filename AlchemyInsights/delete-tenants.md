---
title: 刪除租使用者
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/30/2020
ms.locfileid: "49477655"
---
# <a name="delete-tenant"></a><span data-ttu-id="e2381-102">刪除租使用者</span><span class="sxs-lookup"><span data-stu-id="e2381-102">Delete tenant</span></span>

<span data-ttu-id="e2381-103">若要刪除 Azure AD，請確定：</span><span class="sxs-lookup"><span data-stu-id="e2381-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="e2381-104">您是目錄上的全域系統管理員。</span><span class="sxs-lookup"><span data-stu-id="e2381-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="e2381-105">您未使用具有預設目錄（如 contoso.onmicrosoft.com）的帳戶登入已登入的帳戶，例如 admin@contoso.onmicrosoft.com。</span><span class="sxs-lookup"><span data-stu-id="e2381-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="e2381-106">在刪除之前，移除目錄中的任何使用中應用程式。</span><span class="sxs-lookup"><span data-stu-id="e2381-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="e2381-107">若要移除作用中的應用程式，請流覽至應用程式註冊，並移除現有的應用程式。</span><span class="sxs-lookup"><span data-stu-id="e2381-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="e2381-108">在目錄上沒有任何 Microsoft 線上服務（例如 Microsoft Azure、Office 365 或 Azure AD Premium）的作用中訂閱。</span><span class="sxs-lookup"><span data-stu-id="e2381-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="e2381-109">透過 Azure 支援和帳單轉接您的訂閱或加急取消使用中的訂閱。</span><span class="sxs-lookup"><span data-stu-id="e2381-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="e2381-110">深入瞭解如何取消 Office 365 和 Azure 訂閱。</span><span class="sxs-lookup"><span data-stu-id="e2381-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="e2381-111">如需關聯或將現有訂閱新增至租使用者的指引，請參閱 [關聯或加入 AZURE AD 租使用者的 azure 訂閱](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)。</span><span class="sxs-lookup"><span data-stu-id="e2381-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="e2381-112">沒有主動授權。</span><span class="sxs-lookup"><span data-stu-id="e2381-112">There are no Active license.</span></span> <span data-ttu-id="e2381-113">若要移除授權，請參閱 how [to Remove 訂閱 To remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription)。</span><span class="sxs-lookup"><span data-stu-id="e2381-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="e2381-114">在嘗試刪除 Azure AD 時，在目錄中沒有其他作用中的使用者，而是以全域系統管理員身分。</span><span class="sxs-lookup"><span data-stu-id="e2381-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="e2381-115">移除任何其他作用中的使用者，而且也需要移除租使用者的自訂功能變數名稱上的任何相依性，例如使用 admin@contoso.com 建立的使用者。</span><span class="sxs-lookup"><span data-stu-id="e2381-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="e2381-116">如需更詳細的步驟，請執行下列操作：</span><span class="sxs-lookup"><span data-stu-id="e2381-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="e2381-117">刪除 "Azure Active Directory" 或 "訂閱"，請參閱 [Delete Azure Active directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)。</span><span class="sxs-lookup"><span data-stu-id="e2381-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="e2381-118">移除目錄中的應用程式，請參閱 [移除應用程式](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app)。</span><span class="sxs-lookup"><span data-stu-id="e2381-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
