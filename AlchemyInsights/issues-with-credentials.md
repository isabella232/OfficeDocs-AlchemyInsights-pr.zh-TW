---
title: 認證的問題
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052944"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="5beb0-102">認證的問題</span><span class="sxs-lookup"><span data-stu-id="5beb0-102">Issues with credentials</span></span>

<span data-ttu-id="5beb0-103">[Microsoft identity platform 和 OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 說明如何直接針對 OAuth 2.0 用戶端認證授與流程進行程式設計。</span><span class="sxs-lookup"><span data-stu-id="5beb0-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="5beb0-104">**如何管理應用程式的密碼或憑證認證？**</span><span class="sxs-lookup"><span data-stu-id="5beb0-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="5beb0-105">在 Azure CLI 中，您可以使用 [az ad app 認證](https://docs.microsoft.com/cli/azure/ad/app/credential) 來刪除、列出或重設應用程式的密碼或憑證認證。</span><span class="sxs-lookup"><span data-stu-id="5beb0-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="5beb0-106">**我的使用者如何重設密碼？**</span><span class="sxs-lookup"><span data-stu-id="5beb0-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="5beb0-107">使用者必須先 [註冊自助密碼重設，](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) 才能重設密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="5beb0-108">使用者註冊後，可依照本文中的指示重設密碼： [重設您的工作或學校密碼](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)。</span><span class="sxs-lookup"><span data-stu-id="5beb0-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="5beb0-109">**我的使用者如何變更密碼？**</span><span class="sxs-lookup"><span data-stu-id="5beb0-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="5beb0-110">使用者可以遵循本文中的步驟變更其密碼： [如何變更您的密碼](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)。</span><span class="sxs-lookup"><span data-stu-id="5beb0-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="5beb0-111">他們也可以 [管理兩步驟驗證的應用程式密碼](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)。</span><span class="sxs-lookup"><span data-stu-id="5beb0-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="5beb0-112">**我的使用者在變更或重設其密碼時收到錯誤**</span><span class="sxs-lookup"><span data-stu-id="5beb0-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="5beb0-113">此連結會提供使用者嘗試重設密碼時可能發生的常見問題資訊： [一般問題及其解決方案](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="5beb0-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="5beb0-114">**重設使用者密碼時出現問題**</span><span class="sxs-lookup"><span data-stu-id="5beb0-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="5beb0-115">請確定您有權重設密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="5beb0-116">*只有全域、密碼和使用者管理員才能重設使用者密碼。*</span><span class="sxs-lookup"><span data-stu-id="5beb0-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5beb0-117">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="5beb0-118">請確定您瞭解授權需求：</span><span class="sxs-lookup"><span data-stu-id="5beb0-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="5beb0-119">您的組織中至少必須已指派一個授權：</span><span class="sxs-lookup"><span data-stu-id="5beb0-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="5beb0-120">**僅限雲端使用者** -任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="5beb0-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="5beb0-121">**雲端和/或內部部署使用者** -Azure AD Premium P1 或 P2、Enterprise 可移動性 + SECURITY (EMS) 或安全生產力 (SPE) </span><span class="sxs-lookup"><span data-stu-id="5beb0-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="5beb0-122">若要深入瞭解授權需求，請參閱 [AZURE AD 自助密碼重設的授權需求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)。</span><span class="sxs-lookup"><span data-stu-id="5beb0-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="5beb0-123">若要重設使用者的密碼，請在 Azure AD 中尋找使用者。</span><span class="sxs-lookup"><span data-stu-id="5beb0-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="5beb0-124">然後，在該使用者的 [一覽] 邊欄上，按一下 [重設密碼] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="5beb0-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="5beb0-125">**[密碼重設] 按鈕會灰顯**</span><span class="sxs-lookup"><span data-stu-id="5beb0-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="5beb0-126">您未獲授權，無法重設 **此** 使用者的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="5beb0-127">*只有全域、密碼和使用者管理員才能重設使用者密碼。*</span><span class="sxs-lookup"><span data-stu-id="5beb0-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5beb0-128">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="5beb0-129">**我沒有看到密碼重設的刀片式伺服器**</span><span class="sxs-lookup"><span data-stu-id="5beb0-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="5beb0-130">您未獲授權，無法重設密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="5beb0-131">*只有全域、密碼和使用者管理員才能重設使用者密碼。*</span><span class="sxs-lookup"><span data-stu-id="5beb0-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="5beb0-132">全域管理員也可以重設其他特權管理員的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="5beb0-133">**在密碼重設中看不到內部部署整合刀片式伺服器**</span><span class="sxs-lookup"><span data-stu-id="5beb0-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="5beb0-134">內部部署整合刀片式伺服器只會出現在混合環境中，也就是說，您使用密碼寫回來處理內部部署使用者的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="5beb0-135">在下列情況中看不到此邊欄：</span><span class="sxs-lookup"><span data-stu-id="5beb0-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="5beb0-136">您不是使用密碼回寫</span><span class="sxs-lookup"><span data-stu-id="5beb0-136">You are not using password writeback</span></span>
  - <span data-ttu-id="5beb0-137">密碼寫回的安裝/連線發生問題</span><span class="sxs-lookup"><span data-stu-id="5beb0-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="5beb0-138">Azure AD Connect 的安裝/連線發生問題</span><span class="sxs-lookup"><span data-stu-id="5beb0-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="5beb0-139">如需有關密碼寫回問題的疑難排解步驟，請參閱 [密碼寫回疑難排解](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="5beb0-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="5beb0-140">**我不知道如何重設使用者的密碼**</span><span class="sxs-lookup"><span data-stu-id="5beb0-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="5beb0-141">以適當的系統管理員身分登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="5beb0-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="5beb0-142">移至 [ **使用者和群組** ] 邊欄，選取 [ **所有使用者**]。</span><span class="sxs-lookup"><span data-stu-id="5beb0-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="5beb0-143">從清單中選取使用者。</span><span class="sxs-lookup"><span data-stu-id="5beb0-143">Select a user from the list.</span></span>
4. <span data-ttu-id="5beb0-144">針對選取的使用者，選取 **[概述**]，然後在命令列中選取 [ **重設密碼**]。</span><span class="sxs-lookup"><span data-stu-id="5beb0-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="5beb0-145">選取 [ **重設密碼** ] 按鈕，然後依照畫面上的指示進行。</span><span class="sxs-lookup"><span data-stu-id="5beb0-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="5beb0-146">僅透過 **Azure 入口網站** 支援密碼回寫進行重設。</span><span class="sxs-lookup"><span data-stu-id="5beb0-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="5beb0-147">**我從 Office 365 Admin 入口網站或 Office 365 行動應用程式重設內部部署使用者的密碼，但使用者仍無法登入**</span><span class="sxs-lookup"><span data-stu-id="5beb0-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="5beb0-148">此入口網站不支援密碼回寫。</span><span class="sxs-lookup"><span data-stu-id="5beb0-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="5beb0-149">在 Azure 入口網站中重新重設使用者的密碼。</span><span class="sxs-lookup"><span data-stu-id="5beb0-149">Reset the user's password again in the Azure portal.</span></span>
