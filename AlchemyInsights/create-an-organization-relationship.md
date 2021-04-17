---
title: 建立組織關聯性以允許您的使用者與其他組織共同作業
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816119"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a><span data-ttu-id="36cf1-102">建立組織關聯性以允許您的使用者與其他組織共同作業</span><span class="sxs-lookup"><span data-stu-id="36cf1-102">Create an Organization Relationship to allow your users to collaborate with another organization</span></span>

1. <span data-ttu-id="36cf1-103">從 Microsoft 365 系統管理中心儀表板，移至 [系統管理]  >  [Exchange]。</span><span class="sxs-lookup"><span data-stu-id="36cf1-103">From the Microsoft 365 admin center dashboard, go to **Admin** > **Exchange**.</span></span>
2. <span data-ttu-id="36cf1-104">移至 [組織]  >  [共用]。</span><span class="sxs-lookup"><span data-stu-id="36cf1-104">Go to **organization** > **sharing**.</span></span>
3. <span data-ttu-id="36cf1-105">在 [組織共用] 下，按一下 [新增]。</span><span class="sxs-lookup"><span data-stu-id="36cf1-105">Under **Organization Sharing**, click **New** .</span></span>
4. <span data-ttu-id="36cf1-106">在 [新增組織關聯性] 的 [關聯性名稱] 方塊中，為組織關聯性輸入易記名稱。</span><span class="sxs-lookup"><span data-stu-id="36cf1-106">In **new organization relationship**, in the **Relationship name** box, type a friendly name for the organization relationship.</span></span>
5. <span data-ttu-id="36cf1-107">在 [網域共用對象] 方塊中，輸入想要讓其查看您的行事曆的外部 Office 365 或 Exchange 內部部署組織的網域。</span><span class="sxs-lookup"><span data-stu-id="36cf1-107">In the **Domains to share with** box, type the domain for the external Office 365 or Exchange on-premises organization you want to let see your calendars.</span></span> <span data-ttu-id="36cf1-108">如果您需要輸入多個網域，請使用逗號分隔網域名稱。</span><span class="sxs-lookup"><span data-stu-id="36cf1-108">If you need to enter more than one domain, separate the domain names with a comma.</span></span> <span data-ttu-id="36cf1-109">例如，contoso.com, service.contoso.com。</span><span class="sxs-lookup"><span data-stu-id="36cf1-109">For example, contoso.com, service.contoso.com.</span></span>
6. <span data-ttu-id="36cf1-p102">選取 [啟用行事曆空閒/忙碌資訊共用] 核取方塊，以開啟與您所列之網域的行事曆共用。設定行事曆空閒/忙碌資訊的共用層級，並設定哪些使用者可共用行事曆空閒/忙碌資訊。</span><span class="sxs-lookup"><span data-stu-id="36cf1-p102">Select the **Enable calendar free/busy information sharing** check box to turn on calendar sharing with the domains you listed. Set the sharing level for calendar free/busy information and set which users can share calendar free/busy information.</span></span>  

<span data-ttu-id="36cf1-112">若要設定空閒/忙碌存取層級，請選擇下列其中一項：</span><span class="sxs-lookup"><span data-stu-id="36cf1-112">To set the free/busy access level, select one of the following:</span></span>

- <span data-ttu-id="36cf1-113">**只含時間的行事曆空閒/忙碌資訊**</span><span class="sxs-lookup"><span data-stu-id="36cf1-113">**Calendar free/busy information with time only**</span></span>
- <span data-ttu-id="36cf1-114">**行事曆空閒/忙碌的時間、主題與地點資訊**</span><span class="sxs-lookup"><span data-stu-id="36cf1-114">**Calendar free/busy with time, subject, and location**</span></span>  

 <span data-ttu-id="36cf1-115">若要設定將共用行事曆空閒/忙碌資訊的使用者，請選取下列其中一項：</span><span class="sxs-lookup"><span data-stu-id="36cf1-115">To set which users will share calendar free/busy information, select one of the following:</span></span>

- <span data-ttu-id="36cf1-116">**組織中的所有人**</span><span class="sxs-lookup"><span data-stu-id="36cf1-116">**Everyone in your organization**</span></span>
- <span data-ttu-id="36cf1-117">**指定的安全性群組**</span><span class="sxs-lookup"><span data-stu-id="36cf1-117">**A specified security group**</span></span>  

<span data-ttu-id="36cf1-118">按一下 [瀏覽] 以從清單中挑選安全性群組，然後按一下 [確定]。</span><span class="sxs-lookup"><span data-stu-id="36cf1-118">Click **browse** to pick the security group from a list, then click **ok**.</span></span>

<span data-ttu-id="36cf1-119">按一下 [儲存] 來建立組織關聯性。</span><span class="sxs-lookup"><span data-stu-id="36cf1-119">Click **save** to create the organization relationship.</span></span>  

<span data-ttu-id="36cf1-120">**注意：** 跨租用戶設定不支援個人連絡人的空閒/忙碌查閱。</span><span class="sxs-lookup"><span data-stu-id="36cf1-120">**Note:** Cross-tenant configurations do not support personal contacts for free/busy lookup.</span></span> <span data-ttu-id="36cf1-121">若要讓空閒/忙碌查閱可運作，必須將連絡人包含在全域通訊清單中。</span><span class="sxs-lookup"><span data-stu-id="36cf1-121">Contacts must be included in the global address list for free/busy lookup to work.</span></span>

<span data-ttu-id="36cf1-122">**如需深入了解本主題，請參閱：**</span><span class="sxs-lookup"><span data-stu-id="36cf1-122">**For full understanding of this topic please read:**</span></span>

- [<span data-ttu-id="36cf1-123">在 Exchange Online 中建立組織關聯性</span><span class="sxs-lookup"><span data-stu-id="36cf1-123">Create an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [<span data-ttu-id="36cf1-124">在 Exchange Online 中修改組織關聯性</span><span class="sxs-lookup"><span data-stu-id="36cf1-124">Modify an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [<span data-ttu-id="36cf1-125">在 Exchange Online 中移除組織關聯性</span><span class="sxs-lookup"><span data-stu-id="36cf1-125">Remove an organization relationship in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
