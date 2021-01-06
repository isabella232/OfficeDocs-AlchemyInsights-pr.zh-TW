---
title: 如何新增及管理系統管理員-建議的步驟
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: ed3aa5defabdd4f505ee4f74570023d990910dcb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755826"
---
# <a name="how-to-add-and-manage-administrators---recommended-steps"></a><span data-ttu-id="3c84c-102">如何新增及管理系統管理員-建議的步驟</span><span class="sxs-lookup"><span data-stu-id="3c84c-102">How to add and manage administrators - recommended steps</span></span>

<span data-ttu-id="3c84c-103">根據您的問題描述，我們找到您的解決方案。</span><span class="sxs-lookup"><span data-stu-id="3c84c-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="3c84c-104">當您遵循我們的檔後，大多數客戶都可以自行解決他們的問題。</span><span class="sxs-lookup"><span data-stu-id="3c84c-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="3c84c-105">**編輯訂閱管理員或共同管理員**</span><span class="sxs-lookup"><span data-stu-id="3c84c-105">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="3c84c-106">帳戶管理員可以編輯這兩個角色，而訂閱管理員只能在 [Azure 入口網站](https://ms.portal.azure.com/#home)中變更共同管理員。</span><span class="sxs-lookup"><span data-stu-id="3c84c-106">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="3c84c-107">新增或變更 Azure 訂閱管理員</span><span class="sxs-lookup"><span data-stu-id="3c84c-107">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="3c84c-108">**更新內部 (的訂閱管理員或 Co-Administrator) 訂閱。**</span><span class="sxs-lookup"><span data-stu-id="3c84c-108">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="3c84c-109">服務管理員或共同系統管理員可以使用下列步驟，自行服務此動作：</span><span class="sxs-lookup"><span data-stu-id="3c84c-109">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="3c84c-110">登入 [Azure 入口網站](https://ms.portal.azure.com/#home) ，然後按一下左刀片中的 [ **成本管理 + 帳單** ]。</span><span class="sxs-lookup"><span data-stu-id="3c84c-110">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="3c84c-111">按一下行專案與您的訂閱。</span><span class="sxs-lookup"><span data-stu-id="3c84c-111">Click on the line item with your subscription.</span></span> <span data-ttu-id="3c84c-112">這會開啟您訂閱的概述。</span><span class="sxs-lookup"><span data-stu-id="3c84c-112">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="3c84c-113">在 **訂閱** blade 上，按一下 [ **屬性**]。</span><span class="sxs-lookup"><span data-stu-id="3c84c-113">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="3c84c-114">按一下 [ **服務管理員** ] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="3c84c-114">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="3c84c-115">輸入您要設定為服務管理員之使用者的電子郵件，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="3c84c-115">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="3c84c-116">**新增/變更/移除共同管理員**</span><span class="sxs-lookup"><span data-stu-id="3c84c-116">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="3c84c-117">以服務管理員身分登入 [Azure 入口網站](https://ms.portal.azure.com/#home) 。</span><span class="sxs-lookup"><span data-stu-id="3c84c-117">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="3c84c-118">開啟 [訂閱](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) 並選取訂閱。</span><span class="sxs-lookup"><span data-stu-id="3c84c-118">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="3c84c-119"> (共同管理員只能在訂閱範圍內指派。 ) </span><span class="sxs-lookup"><span data-stu-id="3c84c-119">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="3c84c-120">流覽至 **Access control (IAM)**  >  **傳統系統管理員**  >  **新增**  >  [**新增共同管理員**] 以開啟 [**新增** 共同管理員] 窗格。 (如果 [新增共同管理員] 選項已停用，則表示您沒有) 的許可權。</span><span class="sxs-lookup"><span data-stu-id="3c84c-120">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="3c84c-121">選取您要新增的使用者，然後按一下 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="3c84c-121">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="3c84c-122">**瞭解更多資訊：**</span><span class="sxs-lookup"><span data-stu-id="3c84c-122">**Learn more:**</span></span>
- [<span data-ttu-id="3c84c-123">新增共同管理員</span><span class="sxs-lookup"><span data-stu-id="3c84c-123">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3c84c-124">移除共同管理員</span><span class="sxs-lookup"><span data-stu-id="3c84c-124">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3c84c-125">變更服務管理員</span><span class="sxs-lookup"><span data-stu-id="3c84c-125">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3c84c-126">查看帳戶管理員</span><span class="sxs-lookup"><span data-stu-id="3c84c-126">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="3c84c-127">使用 RBAC 和 Azure 入口網站管理存取權</span><span class="sxs-lookup"><span data-stu-id="3c84c-127">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="3c84c-128">**使用 Azure Active Directory (AD) 新增/刪除使用者**</span><span class="sxs-lookup"><span data-stu-id="3c84c-128">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="3c84c-129">您可以從 Azure Active Directory (Azure AD) 組織中新增或刪除現有的使用者：</span><span class="sxs-lookup"><span data-stu-id="3c84c-129">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="3c84c-130">若要新增使用者，請以組織的使用者管理員身分登入 [Azure 入口網站](https://ms.portal.azure.com/#home) 。</span><span class="sxs-lookup"><span data-stu-id="3c84c-130">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="3c84c-131">選取 [ **Azure Active Directory**]，選取 [ **使用者** ]，然後按一下 [ **新增使用者**]。</span><span class="sxs-lookup"><span data-stu-id="3c84c-131">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="3c84c-132">在 [ **使用者** ] 頁面上，填寫必要的資訊。</span><span class="sxs-lookup"><span data-stu-id="3c84c-132">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="3c84c-133">按一下 [建立 **]**。</span><span class="sxs-lookup"><span data-stu-id="3c84c-133">Click **Create**.</span></span> <span data-ttu-id="3c84c-134">使用者建立並新增至您的 Azure AD 租使用者。</span><span class="sxs-lookup"><span data-stu-id="3c84c-134">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="3c84c-135">**深入瞭解**：</span><span class="sxs-lookup"><span data-stu-id="3c84c-135">**Learn more**:</span></span>

- [<span data-ttu-id="3c84c-136">新增使用者</span><span class="sxs-lookup"><span data-stu-id="3c84c-136">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3c84c-137">刪除使用者</span><span class="sxs-lookup"><span data-stu-id="3c84c-137">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="3c84c-138">使用 Azure Active Directory 新增或更新使用者的設定檔資訊</span><span class="sxs-lookup"><span data-stu-id="3c84c-138">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="3c84c-139">**建議的檔**</span><span class="sxs-lookup"><span data-stu-id="3c84c-139">**Recommended documents**</span></span>

- [<span data-ttu-id="3c84c-140">什麼是以角色為基礎的存取控制 (RBAC) ？</span><span class="sxs-lookup"><span data-stu-id="3c84c-140">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="3c84c-141">瞭解 Azure 中的不同角色</span><span class="sxs-lookup"><span data-stu-id="3c84c-141">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="3c84c-142">Azure Active Directory 中的系統管理員角色權限</span><span class="sxs-lookup"><span data-stu-id="3c84c-142">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="3c84c-143">教學課程：授與使用 RBAC 和 Azure 入口網站的使用者存取</span><span class="sxs-lookup"><span data-stu-id="3c84c-143">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="3c84c-144">疑難排解 Azure 中的 RBAC</span><span class="sxs-lookup"><span data-stu-id="3c84c-144">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="3c84c-145">使用 Azure 管理群組組織資源</span><span class="sxs-lookup"><span data-stu-id="3c84c-145">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="3c84c-146">如何透過電子郵件要求 Azure 發票的副本</span><span class="sxs-lookup"><span data-stu-id="3c84c-146">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="3c84c-147">如何從 Azure 新增、更新或移除信用卡或付款卡</span><span class="sxs-lookup"><span data-stu-id="3c84c-147">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="3c84c-148">管理 (重新啟用/取消/切換) 訂閱</span><span class="sxs-lookup"><span data-stu-id="3c84c-148">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



