---
title: 轉移 Azure 帳單擁有權
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840580"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="cec16-102">轉移 Azure 帳單擁有權</span><span class="sxs-lookup"><span data-stu-id="cec16-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="cec16-103">以擁有要轉移的訂閱的計費帳戶的管理員身份登入到 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="cec16-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="cec16-104">如果不確定您是否是管理員，或者您需要確定是誰，請參閱[確定帳戶計費管理員](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa)。</span><span class="sxs-lookup"><span data-stu-id="cec16-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="cec16-105">在 **成本管理 + 計費** 上搜尋。</span><span class="sxs-lookup"><span data-stu-id="cec16-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="cec16-106">從左方窗格中選取 **訂閱** 。</span><span class="sxs-lookup"><span data-stu-id="cec16-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="cec16-107">依據存取權而定，您可能需要選取計費範圍，然後 **訂閱** 或 **Azure 訂閱** 。</span><span class="sxs-lookup"><span data-stu-id="cec16-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="cec16-108">針對您想要轉移的訂閱，選取 **[轉移帳單擁有權]**</span><span class="sxs-lookup"><span data-stu-id="cec16-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="cec16-109">輸入使用者的電子郵件地址，其為訂閱的新擁有者帳戶的計費管理員，然後選取 **傳送轉移要求**</span><span class="sxs-lookup"><span data-stu-id="cec16-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="cec16-110">使用者會收到一封電子郵件，其中包含檢閱您的轉移要求的指示。</span><span class="sxs-lookup"><span data-stu-id="cec16-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="cec16-111">若要核准轉移要求，使用者會選取電子郵件中的連結，並遵循指示操作。</span><span class="sxs-lookup"><span data-stu-id="cec16-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="cec16-112">**注意事項** ：如果您將您的訂閱帳單擁有權轉移至另一個 Azure AD 租用戶的使用者帳戶，在訂閱中用以管理資源的所有 [角色型存取控制 (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support) 作業皆會永久移除。</span><span class="sxs-lookup"><span data-stu-id="cec16-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="cec16-113">只有新擁有者才有權管理訂閱中的資源。</span><span class="sxs-lookup"><span data-stu-id="cec16-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="cec16-114">如需詳細資訊，請參閱 [將訂閱轉移到另一個 Azure AD 租用戶中的使用者](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="cec16-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="cec16-115">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="cec16-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="cec16-116">轉移 Azure 訂閲帳單擁有權到另一個帳戶</span><span class="sxs-lookup"><span data-stu-id="cec16-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="cec16-117">關於轉移 Azure 訂閱的帳單擁有權</span><span class="sxs-lookup"><span data-stu-id="cec16-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- <span data-ttu-id="cec16-118">[傳送 Visual Studio、Microsoft 合作夥伴網路 (MPN) 和 [預付方案] 開發/測試訂閱](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)</span><span class="sxs-lookup"><span data-stu-id="cec16-118">[Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)</span></span>
- [<span data-ttu-id="cec16-119">轉移擁有權常見問題</span><span class="sxs-lookup"><span data-stu-id="cec16-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="cec16-120">轉移擁有權問題的疑難排解</span><span class="sxs-lookup"><span data-stu-id="cec16-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
