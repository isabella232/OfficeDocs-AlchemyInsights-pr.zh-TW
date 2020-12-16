---
title: 如何新增及管理系統管理員-MCA FL/CL
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2020
ms.locfileid: "49683945"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="f79b4-102">如何新增及管理系統管理員-MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="f79b4-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="f79b4-103">若要管理您的 Microsoft 客戶合約 (MCA) 的帳單帳戶，您可以使用不同的角色與所需的存取層級。</span><span class="sxs-lookup"><span data-stu-id="f79b4-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="f79b4-104">這些角色是除了可協助您控制資源的內建 Azure 服務角色之外的功能。</span><span class="sxs-lookup"><span data-stu-id="f79b4-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="f79b4-105">**若要在 Azure 入口網站中新增計費角色：**</span><span class="sxs-lookup"><span data-stu-id="f79b4-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="f79b4-106">登入 [Azure 入口網站](https://portal.azure.com/)。</span><span class="sxs-lookup"><span data-stu-id="f79b4-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="f79b4-107">搜尋 *成本管理 + 帳單*。</span><span class="sxs-lookup"><span data-stu-id="f79b4-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="f79b4-108">在您想要授與存取權的範圍（例如計費帳戶、計費設定檔或發票區段）上，選取 [Access control (IAM) 。</span><span class="sxs-lookup"><span data-stu-id="f79b4-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="f79b4-109">「存取控制 (IAM) 」頁面會列出指派給該範圍中每個角色的使用者和群組。</span><span class="sxs-lookup"><span data-stu-id="f79b4-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="f79b4-110">若要授與使用者的存取權，請從頁面頂端選取 [ **新增** ]。</span><span class="sxs-lookup"><span data-stu-id="f79b4-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="f79b4-111">在 [ *角色* ] 下拉式清單中，選取角色。</span><span class="sxs-lookup"><span data-stu-id="f79b4-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="f79b4-112">輸入您要授與存取權之使用者的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="f79b4-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="f79b4-113">選取 [ **儲存** ] 以指派角色。</span><span class="sxs-lookup"><span data-stu-id="f79b4-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="f79b4-114">若要移除使用者的存取權，請選取您要移除角色指派的使用者。</span><span class="sxs-lookup"><span data-stu-id="f79b4-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="f79b4-115">選取 [ **移除**]。</span><span class="sxs-lookup"><span data-stu-id="f79b4-115">Select **Remove**.</span></span>

<span data-ttu-id="f79b4-116">**建譯的文件**</span><span class="sxs-lookup"><span data-stu-id="f79b4-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="f79b4-117">計費角色定義</span><span class="sxs-lookup"><span data-stu-id="f79b4-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="f79b4-118">計費帳戶角色和工作</span><span class="sxs-lookup"><span data-stu-id="f79b4-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="f79b4-119">開始使用您的 MCA 計費帳戶</span><span class="sxs-lookup"><span data-stu-id="f79b4-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="f79b4-120">檢查 Microsoft 客戶合約的存取權</span><span class="sxs-lookup"><span data-stu-id="f79b4-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
