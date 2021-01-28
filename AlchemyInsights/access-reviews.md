---
title: 存取權檢查
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7767"
ms.openlocfilehash: b2ba50c4f8e667f81b638ba480fa846e149c3d43
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013927"
---
# <a name="access-reviews"></a><span data-ttu-id="cf136-102">存取權檢查</span><span class="sxs-lookup"><span data-stu-id="cf136-102">Access reviews</span></span>

1. <span data-ttu-id="cf136-103">**啟用存取權檢查**：您可以在建立新的 access 套件或編輯現有的 access 套件時啟用評論。</span><span class="sxs-lookup"><span data-stu-id="cf136-103">**Enable Access Reviews**: You can enable reviews when you create a new access package or edit an existing access package.</span></span> <span data-ttu-id="cf136-104">Create a access package to a [access package In AZURE AD 權利管理](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create)說明如何啟用存取封裝的訪問複查。</span><span class="sxs-lookup"><span data-stu-id="cf136-104">[Create an access review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to enable access reviews of access packages.</span></span>

1. <span data-ttu-id="cf136-105">**檢查存取**： Azure AD 權利管理可簡化企業管理群組、應用程式和 SharePoint 網站的存取。</span><span class="sxs-lookup"><span data-stu-id="cf136-105">**Review Access**: Azure AD entitlement management simplifies how enterprises manage access to groups, applications, and SharePoint sites.</span></span> <span data-ttu-id="cf136-106">[複習 access package to access In AZURE AD 的權利管理](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) 說明如何針對指派給 access 套件的其他使用者，為指定的檢閱者執行訪問複查。</span><span class="sxs-lookup"><span data-stu-id="cf136-106">[Review access of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-create) describes how to perform access reviews for other users that are assigned to an access package as a designated reviewer.</span></span>

1. <span data-ttu-id="cf136-107">**查看您自己的 access**： [在 Azure AD 權利管理中，您可自行複查 access 套件](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) ，說明使用者如何對其所指派的 Access 套件進行自我審閱 (s) 。</span><span class="sxs-lookup"><span data-stu-id="cf136-107">**Review Access for Yourself**: [Self-review of an access package in Azure AD entitlement management](https://docs.microsoft.com/azure/active-directory/governance/entitlement-management-access-reviews-self-review) describes how a user does a self-review of their assigned access package(s).</span></span>

1. <span data-ttu-id="cf136-108">在大多數情況下，使用者會在 [ **存取面板**] 中找到等候其回應的複查。</span><span class="sxs-lookup"><span data-stu-id="cf136-108">In most cases, end users will find a review pending their response in the **Access Panel**.</span></span> <span data-ttu-id="cf136-109">這只適用于群組和應用程式的評論，不適用於角色。</span><span class="sxs-lookup"><span data-stu-id="cf136-109">This is only applicable to reviews of Groups and Applications, not Roles.</span></span> <span data-ttu-id="cf136-110">針對角色的所有訪問檢查，使用者必須流覽至 Azure AD 特權身分識別管理 (PIM) 以完成其複查。</span><span class="sxs-lookup"><span data-stu-id="cf136-110">For all Access Reviews of roles, end users must navigate to Azure AD Privileged Identity Management (PIM) to complete their review.</span></span>

    1. <span data-ttu-id="cf136-111">登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="cf136-111">Logon to the Azure portal.</span></span>
    2. <span data-ttu-id="cf136-112">流覽至 Azure AD PIM。</span><span class="sxs-lookup"><span data-stu-id="cf136-112">Navigate to Azure AD PIM.</span></span>
    3. <span data-ttu-id="cf136-113">在左功能窗格中，選取 [**任務**  >  **檢查存取**]。</span><span class="sxs-lookup"><span data-stu-id="cf136-113">In the left navigation pane, select **Tasks** > **Review access**.</span></span>
    
<span data-ttu-id="cf136-114">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="cf136-114">For more information, see:</span></span>

- [<span data-ttu-id="cf136-115">在 PIM 中執行我 Azure AD 目錄角色的存取檢查 </span><span class="sxs-lookup"><span data-stu-id="cf136-115">Perform an access review of my Azure AD directory roles in PIM </span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-perform-security-review/)
- [<span data-ttu-id="cf136-116">在 PIM 中執行 my Azure 資源角色的存取檢查</span><span class="sxs-lookup"><span data-stu-id="cf136-116">Perform an access review of my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-perform-access-review/)