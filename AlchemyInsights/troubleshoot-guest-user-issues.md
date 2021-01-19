---
title: 對來賓使用者問題進行疑難排解
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004358"
- "7822"
ms.openlocfilehash: 0f2a10b918fee067b167ab58ac2544a89e0c8ea1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49897695"
---
# <a name="troubleshoot-guest-user-issues"></a><span data-ttu-id="d695f-102">對來賓使用者問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="d695f-102">Troubleshoot guest user issues</span></span>

1. <span data-ttu-id="d695f-103">如需管理對應用程式之來賓存取的指導方針，請參閱 [Manage guest access With AZURE AD access 評論](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews)。</span><span class="sxs-lookup"><span data-stu-id="d695f-103">For guidance on managing guest access to applications, see [Manage guest access with Azure AD access reviews](https://docs.microsoft.com/azure/active-directory/governance/manage-guest-access-with-access-reviews).</span></span>
1. <span data-ttu-id="d695f-104">在[azure 入口網站中將來賓使用者新增至您的目錄](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal)：在此快速入門中，您將透過 azure 入口網站將新的來賓使用者新增至 azure AD 目錄、傳送邀請，以及查看來賓使用者的邀請兌換處理常式的外觀。</span><span class="sxs-lookup"><span data-stu-id="d695f-104">[Add guest users to your directory in the Azure portal](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal): In this quickstart, you'll add a new guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's invitation redemption process looks like.</span></span>
1. <span data-ttu-id="d695f-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell)：在此快速入門中，您將使用 New-AzureADMSInvitation 命令，將一個來賓使用者新增至您的 Azure 租使用者。</span><span class="sxs-lookup"><span data-stu-id="d695f-105">[Add a guest user with PowerShell](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-invite-powershell): In this quickstart, you’ll use the New-AzureADMSInvitation command to add one guest user to your Azure tenant.</span></span>
1. <span data-ttu-id="d695f-106">若要瞭解如何將使用者和群組指派給 Azure Active Directory 中的企業應用程式 (Azure AD) （從 Azure 入口網站或使用 PowerShell），請參閱在 [Azure Active directory 中管理應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)。</span><span class="sxs-lookup"><span data-stu-id="d695f-106">To learn how to assign users, and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span> 
1. <span data-ttu-id="d695f-107">Azure Active Directory (Azure AD) B2B 共同作業可搭配大多數與 Azure AD 整合的應用程式使用。</span><span class="sxs-lookup"><span data-stu-id="d695f-107">Azure Active Directory (Azure AD) B2B collaboration works with most apps that integrate with Azure AD.</span></span> <span data-ttu-id="d695f-108">在 [本文](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps)中，我們將逐步逐步說明如何設定一些流行的 SaaS 應用程式，以搭配 Azure AD B2B 使用。</span><span class="sxs-lookup"><span data-stu-id="d695f-108">In this [article](https://docs.microsoft.com/azure/active-directory/external-identities/configure-saas-apps), we walk through instructions for configuring some popular SaaS apps for use with Azure AD B2B.</span></span>
1. <span data-ttu-id="d695f-109">使用 Azure Active Directory (Azure AD) B2B 共同作業功能，將來賓使用者從夥伴組織邀請至您的 Azure AD 的組織，您現在可以提供這些 B2B 使用者對內部部署應用程式的存取權。</span><span class="sxs-lookup"><span data-stu-id="d695f-109">As an organization that uses Azure Active Directory (Azure AD) B2B collaboration capabilities to invite guest users from partner organizations to your Azure AD, you can now provide these B2B users access to on-premises apps.</span></span> <span data-ttu-id="d695f-110">這些內部部署應用程式可以使用 SAML-based 驗證或整合式 Windows 驗證 (IWA) 與 Kerberos 限制委派 (KCD) 。</span><span class="sxs-lookup"><span data-stu-id="d695f-110">These on-premises apps can use SAML-based authentication or Integrated Windows Authentication (IWA) with Kerberos constrained delegation (KCD).</span></span> <span data-ttu-id="d695f-111">如需詳細資訊，請參閱在 [AZURE AD 中授與 B2B 使用者內部部署應用程式的存取權](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises)。</span><span class="sxs-lookup"><span data-stu-id="d695f-111">For more information, see [Grant B2B users in Azure AD access to your on-premises applications](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-cloud-to-on-premises).</span></span>
1. <span data-ttu-id="d695f-112">瞭解如何 [使用 AZURE AD B2B 共同作業，授與受管理的本機夥伴帳戶對雲端資源的存取權](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud)。</span><span class="sxs-lookup"><span data-stu-id="d695f-112">Learn how to [grant locally-managed partner accounts access to cloud resources using Azure AD B2B collaboration](https://docs.microsoft.com/azure/active-directory/external-identities/hybrid-on-premises-to-cloud).</span></span>