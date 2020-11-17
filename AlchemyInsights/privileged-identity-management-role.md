---
title: 特權身分識別管理角色
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
- "9003230"
- "6825"
ms.openlocfilehash: 726511d016462f56c48a4272b57abc3e9f0cbc3d
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086283"
---
# <a name="privileged-identity-managementpim-role"></a><span data-ttu-id="c416b-102"> (PIM) 角色的特權身分識別管理</span><span class="sxs-lookup"><span data-stu-id="c416b-102">Privileged Identity Management(PIM) role</span></span>

<span data-ttu-id="c416b-103">**啟用角色之後未授與許可權**</span><span class="sxs-lookup"><span data-stu-id="c416b-103">**Permissions are not granted after activating a role**</span></span>

<span data-ttu-id="c416b-104">當您在 Azure AD 特權身分識別管理 (PIM) 中啟動角色時，啟用可能不會立即傳播至需要許可權角色的所有入口網站。</span><span class="sxs-lookup"><span data-stu-id="c416b-104">When you activate a role in Azure AD Privileged Identity Management (PIM), the activation may not instantly propagate to all portals that require the privileged role.</span></span> <span data-ttu-id="c416b-105">有時候，即使變更遭到傳播，在入口網站中的 web 快取可能會導致變更不會立即生效。</span><span class="sxs-lookup"><span data-stu-id="c416b-105">Sometimes, even if the change is propagated, web caching in a portal may result in the change not taking effect immediately.</span></span>

<span data-ttu-id="c416b-106">如果您的啟用延遲，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c416b-106">If your activation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="c416b-107">登出 Azure 入口網站，然後重新登入。</span><span class="sxs-lookup"><span data-stu-id="c416b-107">Sign out of the Azure portal and then sign back in.</span></span> <span data-ttu-id="c416b-108">當您啟動 Azure AD 角色或 Azure 資源角色時，您將會看到您的啟用階段。</span><span class="sxs-lookup"><span data-stu-id="c416b-108">When you activate an Azure AD role or an Azure resource role, you will see the stages of your activation.</span></span> <span data-ttu-id="c416b-109">完成所有階段後，您將會看到「登出」連結。</span><span class="sxs-lookup"><span data-stu-id="c416b-109">Once all the stages are complete, you will see a 'Sign out' link.</span></span> <span data-ttu-id="c416b-110">您可以使用此連結登出。這會解決啟用延遲的大部分案例。</span><span class="sxs-lookup"><span data-stu-id="c416b-110">You can use this link to sign out. This will solve most cases for activation delay.</span></span>
2. <span data-ttu-id="c416b-111">在 PIM 中，確認您已列為該角色的成員。</span><span class="sxs-lookup"><span data-stu-id="c416b-111">In PIM, verify that you are listed as the member of the role.</span></span>
3. <span data-ttu-id="c416b-112">如果您要啟用 Exchange 系統管理員角色，請確定登出後再重新登入。</span><span class="sxs-lookup"><span data-stu-id="c416b-112">If you are activating the Exchange Administrator role, make sure you sign out and sign back in.</span></span> <span data-ttu-id="c416b-113">如果問題持續發生，請開啟支援票證，並將此問題當做問題提出。</span><span class="sxs-lookup"><span data-stu-id="c416b-113">If the problem persists, open a support ticket and raise this as an issue.</span></span> <span data-ttu-id="c416b-114">如果您使用 Exchange 系統管理員角色來存取安全性與合規性中心，請參閱下一個步驟。</span><span class="sxs-lookup"><span data-stu-id="c416b-114">If you are using your Exchange Administrator role to access the Security and Compliance Center, see the next step.</span></span>
4. <span data-ttu-id="c416b-115">如果您要啟用角色以存取安全性與合規性中心，或是若要啟用 SharePoint 系統管理員角色，您會在幾分鐘內經歷幾分鐘內的啟動延遲。</span><span class="sxs-lookup"><span data-stu-id="c416b-115">If you are activating a role to access the Security and Compliance Center or if you are activating the SharePoint Administrator role, you will experience some activation delay from a few minutes up to a few hours.</span></span> <span data-ttu-id="c416b-116">這是已知的問題，我們積極與這些小組合作，盡可能立即解決此問題。</span><span class="sxs-lookup"><span data-stu-id="c416b-116">This is a known issue and we are actively working with these teams to resolve this issue as soon as possible.</span></span>

<span data-ttu-id="c416b-117">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="c416b-117">For more information, see:</span></span>

- [<span data-ttu-id="c416b-118">啟動我的 Azure AD role in PIM</span><span class="sxs-lookup"><span data-stu-id="c416b-118">Activate my Azure AD roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "HTTPs://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [<span data-ttu-id="c416b-119">以 PIM 啟用我的 Azure 資源角色</span><span class="sxs-lookup"><span data-stu-id="c416b-119">Activate my Azure resource roles in PIM</span></span>](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "HTTPs://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

<span data-ttu-id="c416b-120">**停用角色或角色啟用到期後，不會移除許可權**</span><span class="sxs-lookup"><span data-stu-id="c416b-120">**Permissions are not removed after deactivating a role or the role activation expires**</span></span>

<span data-ttu-id="c416b-121">當您停用 Azure AD 特權身分識別管理中的角色或角色啟用期限到期時，可能會發生延遲，讓您繼續存取。</span><span class="sxs-lookup"><span data-stu-id="c416b-121">When you deactivate a role in Azure AD Privileged Identity Management or when a role activation period expires, there might be a delay where you continue to have access.</span></span>

<span data-ttu-id="c416b-122">如果停用延遲，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c416b-122">If your deactivation is delayed, follow these steps:</span></span>

1. <span data-ttu-id="c416b-123">如果您停用 Exchange 系統管理員角色或角色啟用期限已到期，而且在移除許可權之前發現明顯的延遲，請開啟支援票證，並告知您的支援工程師，以協助您使用「特權存取管理」 (PAM) 小組（如有關于此問題的 Office）進行票證的檔。</span><span class="sxs-lookup"><span data-stu-id="c416b-123">If you are deactivating the Exchange Administrator role or the role activation period expires, and you notice a significant delay before the permissions are removed, open a support ticket and tell your support engineer to help you file a ticket with the Privileged Access Management (PAM) team inside Office about this issue.</span></span>
2. <span data-ttu-id="c416b-124">如果啟用期限已到期，但您仍已開啟瀏覽器會話，請關閉瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="c416b-124">If the activation period has expired, but you still have the browser session open, close your browser.</span></span> <span data-ttu-id="c416b-125">您可以繼續使用角色，直到您關閉該會話為止。</span><span class="sxs-lookup"><span data-stu-id="c416b-125">You can continue to use the role until you close that session.</span></span> <span data-ttu-id="c416b-126">這是已知的問題，當啟用已到期時，我們就會查看每個會話的潛在修正會主動吊銷。</span><span class="sxs-lookup"><span data-stu-id="c416b-126">This is a known issue and we are looking at a potential fix to actively revoke each session once activation has expired.</span></span>

<span data-ttu-id="c416b-127">如果您的延遲與這兩個案例不同，請開啟支援票證。</span><span class="sxs-lookup"><span data-stu-id="c416b-127">If your delay is different than these two scenarios, please open a support ticket.</span></span>
