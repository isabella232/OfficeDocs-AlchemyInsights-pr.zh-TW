---
title: 重設密碼時的問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50585649"
---
# <a name="problems-resetting-password"></a><span data-ttu-id="33930-102">重設密碼時的問題</span><span class="sxs-lookup"><span data-stu-id="33930-102">Problems resetting password</span></span>

<span data-ttu-id="33930-103">以下是重設密碼及可能的解決方案時可能面臨的一些問題：</span><span class="sxs-lookup"><span data-stu-id="33930-103">Following are some of the issues that you might face when resetting password and the possible solutions:</span></span>

<span data-ttu-id="33930-104">**我遇到其他類別未涵蓋的密碼重設問題**</span><span class="sxs-lookup"><span data-stu-id="33930-104">**I'm having an issue with password reset not covered in the other categories**</span></span>

- <span data-ttu-id="33930-105">確定您有權重設密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-105">Ensure you are authorized to reset passwords.</span></span> <span data-ttu-id="33930-106">只有全域、密碼和使用者管理員才能重設使用者密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-106">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="33930-107">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-107">Global administrators can also reset other privileged administrator's passwords.</span></span>
- <span data-ttu-id="33930-108">確定您瞭解授權需求：</span><span class="sxs-lookup"><span data-stu-id="33930-108">Ensure that you understand the licensing requirements:</span></span>
    - <span data-ttu-id="33930-109">您的組織中必須至少有一個指派的授權</span><span class="sxs-lookup"><span data-stu-id="33930-109">You must have at least one license assigned in your organization</span></span>
        - <span data-ttu-id="33930-110">僅限雲端使用者-任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="33930-110">Cloud only users - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
        - <span data-ttu-id="33930-111">雲端和/或內部部署使用者-Azure AD Premium P1 或 P2、Enterprise 可移動性 + Security (EMS) 或安全生產力 (SPE) </span><span class="sxs-lookup"><span data-stu-id="33930-111">Cloud and/or on-premises users - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
        - <span data-ttu-id="33930-112">若要閱讀授權要求的詳細資訊，請參閱 [Microsoft AZURE AD 自助密碼重設的授權需求一](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)文。</span><span class="sxs-lookup"><span data-stu-id="33930-112">To read more about licensing requirements see the article [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="33930-113">**我在測試設定的密碼重設原則時發生問題**</span><span class="sxs-lookup"><span data-stu-id="33930-113">**I'm having problems testing the password reset policy I set**</span></span>

- <span data-ttu-id="33930-114">最近套用的原則可能需要數分鐘的時間才能跨所有資料中心和端點進行複製。</span><span class="sxs-lookup"><span data-stu-id="33930-114">Recently applied policies can take several minutes to replicate across all data centers and end-points.</span></span> <span data-ttu-id="33930-115">從資料中心的實體距離也會影響套用變更的速度。</span><span class="sxs-lookup"><span data-stu-id="33930-115">Physical distance from the data center will also affect how quickly changes are applied.</span></span>
- <span data-ttu-id="33930-116">與使用者進行測試，而不是以系統管理員的身分進行測試，而是一小組使用者的試驗。</span><span class="sxs-lookup"><span data-stu-id="33930-116">Test with an end user, not an administrator, and pilot with a small set of users.</span></span> <span data-ttu-id="33930-117">在 Azure 入口網站中設定的原則只適用于使用者，而非系統管理員。</span><span class="sxs-lookup"><span data-stu-id="33930-117">The policies configured in the Azure portal ONLY apply to end-users, not administrators.</span></span> <span data-ttu-id="33930-118">Microsoft 對任何 Azure 系統管理員角色強制實施強預設雙門密碼重設原則 (例如：全域系統管理員、服務台管理員、密碼管理員等 ) </span><span class="sxs-lookup"><span data-stu-id="33930-118">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role (Example: Global Administrator, Helpdesk Administrator, Password Administrator, etc.)</span></span>
    - <span data-ttu-id="33930-119">深入瞭解系統 [管理員的原則](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)。</span><span class="sxs-lookup"><span data-stu-id="33930-119">Learn more about [policies for administrators](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences).</span></span>

<span data-ttu-id="33930-120">**我想要部署密碼重設，但不想讓使用者註冊其他安全性資訊**</span><span class="sxs-lookup"><span data-stu-id="33930-120">**I want to deploy password reset but I don't want to make my users register additional security info**</span></span>

<span data-ttu-id="33930-121">預先填入使用者的資料，使其不需要！</span><span class="sxs-lookup"><span data-stu-id="33930-121">Pre-populate data for your users so they don't have to!</span></span> <span data-ttu-id="33930-122">-以系統管理員的身分，您可以設定使用者的電話和電子郵件內容，然後再將密碼重設為您的組織。</span><span class="sxs-lookup"><span data-stu-id="33930-122">- As an administrator you can set phone and email properties for your users before rolling out password reset to your organization.</span></span> <span data-ttu-id="33930-123">您可以使用 API、PowerShell 或 Azure AD Connect 來執行此動作。</span><span class="sxs-lookup"><span data-stu-id="33930-123">You can do this using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="33930-124">其他資訊：</span><span class="sxs-lookup"><span data-stu-id="33930-124">More information here:</span></span>
- [<span data-ttu-id="33930-125">部署密碼重設，但不需要使用者註冊</span><span class="sxs-lookup"><span data-stu-id="33930-125">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [<span data-ttu-id="33930-126">密碼重設所使用的資料</span><span class="sxs-lookup"><span data-stu-id="33930-126">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="33930-127">**[密碼重設] 按鈕會灰顯**</span><span class="sxs-lookup"><span data-stu-id="33930-127">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="33930-128">您未獲授權，無法重設此使用者的密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-128">You are not authorized to reset this user's passwords.</span></span> <span data-ttu-id="33930-129">只有全域、密碼和使用者管理員才能重設使用者密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-129">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="33930-130">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-130">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="33930-131">**我沒有看到密碼重設的刀片式伺服器**</span><span class="sxs-lookup"><span data-stu-id="33930-131">**I don't see the password reset blade**</span></span>

<span data-ttu-id="33930-132">您未獲授權，無法重設密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-132">You are not authorized to reset passwords.</span></span> <span data-ttu-id="33930-133">只有全域、密碼和使用者管理員才能重設使用者密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-133">Only global, password, and user administrators can reset user passwords.</span></span> <span data-ttu-id="33930-134">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-134">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="33930-135">**在密碼重設中看不到內部部署整合刀片式伺服器**</span><span class="sxs-lookup"><span data-stu-id="33930-135">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="33930-136">內部部署整合刀片式伺服器只會出現在混合環境中，也就是說，您使用密碼寫回來處理內部部署使用者的密碼。</span><span class="sxs-lookup"><span data-stu-id="33930-136">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>
- <span data-ttu-id="33930-137">在下列情況中看不到此邊欄：</span><span class="sxs-lookup"><span data-stu-id="33930-137">You do not see this blade if:</span></span>
    - <span data-ttu-id="33930-138">您不是使用密碼回寫</span><span class="sxs-lookup"><span data-stu-id="33930-138">You are not using password writeback</span></span>
    - <span data-ttu-id="33930-139">密碼寫回的安裝/連線發生問題</span><span class="sxs-lookup"><span data-stu-id="33930-139">There is a problem with your installation/connectivity of password writeback</span></span>
    - <span data-ttu-id="33930-140">Azure AD Connect 的安裝/連線發生問題</span><span class="sxs-lookup"><span data-stu-id="33930-140">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
    - <span data-ttu-id="33930-141">如需有關密碼寫回問題的疑難排解步驟，請參閱[密碼寫回疑難排解](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)一節。</span><span class="sxs-lookup"><span data-stu-id="33930-141">For more troubleshooting steps for issues with password writeback, see the section [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="33930-142">**我不知道如何重設使用者的密碼**</span><span class="sxs-lookup"><span data-stu-id="33930-142">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="33930-143">以適當的系統管理員身分登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="33930-143">Sign in to the Azure portal as an appropriate admin.</span></span>
1. <span data-ttu-id="33930-144">移至 [使用者和群組] 邊欄，選取 [ **所有使用者**]。</span><span class="sxs-lookup"><span data-stu-id="33930-144">Go to the Users and groups blade, select **All Users**.</span></span>
1. <span data-ttu-id="33930-145">從清單中選取使用者。</span><span class="sxs-lookup"><span data-stu-id="33930-145">Select a user from the list.</span></span>
1. <span data-ttu-id="33930-146">針對選取的使用者，選取 **[概述**]，然後在命令列中，按一下 [ **重設密碼**]。</span><span class="sxs-lookup"><span data-stu-id="33930-146">For the selected user, select **Overview**, and then in the command bar, click **Reset password**.</span></span>
1. <span data-ttu-id="33930-147">依照畫面上的指示進行。</span><span class="sxs-lookup"><span data-stu-id="33930-147">Follow the instructions on the screen.</span></span>
    - <span data-ttu-id="33930-148">僅透過 Azure 入口網站支援密碼回寫進行重設。</span><span class="sxs-lookup"><span data-stu-id="33930-148">Only resets performed through the Azure portal support password writeback.</span></span>

<span data-ttu-id="33930-149">**我從 Office 365 Admin 入口網站或 Office 365 行動應用程式重設內部部署使用者的密碼，但使用者仍無法登入**</span><span class="sxs-lookup"><span data-stu-id="33930-149">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="33930-150">此入口網站不支援密碼回寫。</span><span class="sxs-lookup"><span data-stu-id="33930-150">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="33930-151">在 Azure 入口網站中重新重設使用者的密碼 portal.azure.com</span><span class="sxs-lookup"><span data-stu-id="33930-151">Reset the user's password again in the Azure portal - portal.azure.com</span></span>

