---
title: 支援的訂閱類型
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
- "9003560"
- "6675"
ms.openlocfilehash: dcf5855bff8725ea746196c1f07d689ce1797f8c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820673"
---
# <a name="supported-subscription-types"></a><span data-ttu-id="006ca-102">支援的訂閱類型</span><span class="sxs-lookup"><span data-stu-id="006ca-102">Supported subscription types</span></span>

<span data-ttu-id="006ca-103">請查看支援的訂閱類型以繼續進行。</span><span class="sxs-lookup"><span data-stu-id="006ca-103">Please review the supported subscription types to proceed further.</span></span>

[<span data-ttu-id="006ca-104">支援的訂閱類型</span><span class="sxs-lookup"><span data-stu-id="006ca-104">Supported subscription types</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#supported-subscription-types)

<span data-ttu-id="006ca-105">**轉移帳單擁有權**</span><span class="sxs-lookup"><span data-stu-id="006ca-105">**Transfer billing ownership**</span></span>

<span data-ttu-id="006ca-106">[Microsoft Azure 入口網站] 為計費帳戶的 [帳戶系統管理員](https://ms.portal.azure.com/)，該帳戶含有您想要轉移的訂閱</span><span class="sxs-lookup"><span data-stu-id="006ca-106">Azure portal as the [Account Admin](https://ms.portal.azure.com/) of the billing account that has the subscription you want to transfer</span></span>

- <span data-ttu-id="006ca-107">在 **成本管理 + 計費** 上搜尋。</span><span class="sxs-lookup"><span data-stu-id="006ca-107">Search on **Cost Management + Billing**.</span></span> <span data-ttu-id="006ca-108">從左方窗格中選取 **訂閱**。</span><span class="sxs-lookup"><span data-stu-id="006ca-108">Select **Subscriptions** from left-pane.</span></span> <span data-ttu-id="006ca-109">依據存取權而定，您可能需要選取計費範圍，然後 **訂閱** 或 **Azure 訂閱**。</span><span class="sxs-lookup"><span data-stu-id="006ca-109">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="006ca-110">針對您想要轉移的訂閱，選取 [轉移帳單擁有權]</span><span class="sxs-lookup"><span data-stu-id="006ca-110">Select Transfer billing ownership for the subscription you want to transfer</span></span>
- <span data-ttu-id="006ca-111">輸入使用者的電子郵件地址，其為訂閱的新擁有者帳戶的計費管理員，然後選取 **傳送轉移要求**</span><span class="sxs-lookup"><span data-stu-id="006ca-111">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="006ca-112">使用者會收到一封電子郵件，其中包含檢閱您的轉移要求的指示。</span><span class="sxs-lookup"><span data-stu-id="006ca-112">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="006ca-113">若要核准轉移要求，使用者會選取電子郵件中的連結，並遵循指示操作。</span><span class="sxs-lookup"><span data-stu-id="006ca-113">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="006ca-114">注意事項：如果您將您的訂閱帳單擁有權轉移至另一個 Azure AD 租用戶的使用者帳戶，在訂閱中用以管理資源的所有 [角色型存取控制 (RBAC) ](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)作業皆會永久移除。</span><span class="sxs-lookup"><span data-stu-id="006ca-114">Note: If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="006ca-115">只有新擁有者才有權管理訂閱中的資源。</span><span class="sxs-lookup"><span data-stu-id="006ca-115">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="006ca-116">如需詳細資訊，請參閱 [將訂閱轉移到另一個 Azure AD 租用戶中的使用者](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="006ca-116">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="006ca-117">**轉移訂閱的擁有權**</span><span class="sxs-lookup"><span data-stu-id="006ca-117">**Transfer Ownership of Subscription**</span></span>

<span data-ttu-id="006ca-118">[訂閱擁有者轉移] 必須有角色型存取控制(RBAC) 以管理訂閱中的資源失去其存取權。</span><span class="sxs-lookup"><span data-stu-id="006ca-118">Subscription Ownership Transfer prerequisites role based access (RBAC) to manage resources in the subscription lose their access.</span></span> <span data-ttu-id="006ca-119">如需有關將現有的訂閱新增至租用戶的詳細資訊，請參閱 [關聯或新增一個 Azure 訂閱至 Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="006ca-119">For more information about adding an existing subscription to a tenant, see [Associate or add an Azure subscription to Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

- <span data-ttu-id="006ca-120">在目前計費週期中有現有未付金額的 [訂閱轉移] ，將不會轉移到新帳戶的新付款方式。</span><span class="sxs-lookup"><span data-stu-id="006ca-120">Subscription Transfer with an existing outstanding amount from the current billing cycle will not be transferred to the new payment instrument in the new account.</span></span> <span data-ttu-id="006ca-121">新帳戶使用者唯一能使用的資訊只有上個月的訂閱費用。</span><span class="sxs-lookup"><span data-stu-id="006ca-121">The only information available to the users in new account is the last month's cost for your subscription.</span></span> <span data-ttu-id="006ca-122">其餘的使用和計費記錄都不會隨訂閱轉移。</span><span class="sxs-lookup"><span data-stu-id="006ca-122">The rest of the usage and billing history does not transfer with the subscription.</span></span>
- <span data-ttu-id="006ca-123">Enterprise 合約 (EA) 訂閱的 [轉移帳單擁有權] 目前僅在 Enterprise 合約入口網站中支援。</span><span class="sxs-lookup"><span data-stu-id="006ca-123">Transfer billing ownership of Enterprise Agreement (EA) subscriptions is currently supported in the Enterprise Agreement Portal only</span></span>
- <span data-ttu-id="006ca-124">將信用卡級訂閱 (例如 Visual Studio、BizSpark、Microsoft 合作夥伴網路) 轉移到新的使用者，需要有 Visual Studio/Microsoft 合作夥伴網路授權才能接受轉移要求</span><span class="sxs-lookup"><span data-stu-id="006ca-124">Transferring a credit-oriented subscription like Visual Studio, BizSpark, Microsoft Partner Network to a new user requires to have a Visual Studio/Microsoft partner network license to accept the transfer request</span></span>
- <span data-ttu-id="006ca-125">所有的資源像是虛擬機器、磁碟和網站成功地轉移到新帳戶。</span><span class="sxs-lookup"><span data-stu-id="006ca-125">All resources like Virtual Machines, disks, and websites transfer to the new account successfully.</span></span> <span data-ttu-id="006ca-126">在跨租用戶的訂閱轉移中，下列資源可能會受到影響：</span><span class="sxs-lookup"><span data-stu-id="006ca-126">The following resources could be affected in a cross-tenant subscription transfer:</span></span>

<span data-ttu-id="006ca-127">**Azure AD Domain Services**</span><span class="sxs-lookup"><span data-stu-id="006ca-127">**Azure AD Domain Services**</span></span>

<span data-ttu-id="006ca-128">Azure Key Vaults</span><span class="sxs-lookup"><span data-stu-id="006ca-128">Azure Key Vaults</span></span>

- <span data-ttu-id="006ca-129">[SQL 相關使用者和資料庫](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) 可能會受到影響，特別是如果客戶使用 Azure Active Directory 相關的驗證</span><span class="sxs-lookup"><span data-stu-id="006ca-129">[SQL related users and databases](https://docs.microsoft.com/azure/sql-database/sql-database-aad-authentication-configure?WT.mc_id=Portal-Microsoft_Azure_Support) could be impacted, especially if the customer uses an Azure Active Directory related authentication</span></span>
- <span data-ttu-id="006ca-130">使用 Azure Active Directory 驗證設定的 **應用程式服務** 可能會受到影響</span><span class="sxs-lookup"><span data-stu-id="006ca-130">**App Services** configured with Azure Active Directory authentication could be impacted</span></span>
- <span data-ttu-id="006ca-131">當已連結的 Azure 訂閱取消時，已連線到 Azure 訂閱的 **Visual Studio Team** 服務帳戶可能會暫時無法存取。</span><span class="sxs-lookup"><span data-stu-id="006ca-131">**Visual Studio Team** Services accounts connected to Azure subscriptions may temporarily lose access when the connected Azure subscription is cancelled</span></span>

<span data-ttu-id="006ca-132">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="006ca-132">**Recommended Documents**</span></span>

<span data-ttu-id="006ca-133">接受帳單擁有權之後的步驟：</span><span class="sxs-lookup"><span data-stu-id="006ca-133">Steps after accepting billing ownership:</span></span>

- <span data-ttu-id="006ca-134">若要保留帳單擁有權，但變更您的訂閱類型，請參照：[將您的 Azure 訂閱切換到其他方案](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="006ca-134">To retain billing ownership, but change the type of your subscription, refer: [Switch your Azure subscription to another offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="006ca-135">[傳送 Visual Studio、Microsoft 合作夥伴網路 (MPN) 和 [預付方案] 開發/測試訂閱](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="006ca-135">[Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)</span></span>
- <span data-ttu-id="006ca-136">[[企業合約 (EA)] 訂閱的轉移帳單擁有權](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="006ca-136">[Transfer billing ownership of Enterprise Agreement (EA) subscriptions](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transfer-billing-ownership-of-enterprise-agreement-ea-subscriptions)</span></span>
- [<span data-ttu-id="006ca-137">轉移擁有權常見問題</span><span class="sxs-lookup"><span data-stu-id="006ca-137">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="006ca-138">轉移擁有權問題的疑難排解</span><span class="sxs-lookup"><span data-stu-id="006ca-138">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)