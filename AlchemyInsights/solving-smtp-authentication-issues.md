---
title: 啟用 SMTP 驗證和疑難排解
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
- "3000003"
- "5652"
ms.openlocfilehash: 4695a2f111823739c4d87fa2b262a5e64e080955
ms.sourcegitcommit: 2103d706492ad7ee9596344714c0520569ebd6af
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/23/2021
ms.locfileid: "53077642"
---
# <a name="enable-smtp-authentication-and-troubleshooting"></a><span data-ttu-id="583ca-102">啟用 SMTP 驗證和疑難排解</span><span class="sxs-lookup"><span data-stu-id="583ca-102">Enable SMTP authentication and troubleshooting</span></span>

<span data-ttu-id="583ca-103">如果您想要為信箱啟用 SMTP 驗證，或您在嘗試向 Microsoft 365 驗證裝置或應用程式來轉送電子郵件時，遇到代碼為 5.7.57 或 5.7.3 或 5.7.139 的「用戶端未驗證」、「驗證失敗」或 "SmtpClientAuthentication" 錯誤，請執行這三個動作以解決問題：</span><span class="sxs-lookup"><span data-stu-id="583ca-103">If you want to enable SMTP authentication for a mailbox or you're getting a "Client not authenticated", "Authentication unsuccessful", or "SmtpClientAuthentication" error with code 5.7.57 or 5.7.3 or 5.7.139 when you try to relay email by authenticating a device or application with Microsoft 365, perform these three actions to resolve the issue:</span></span>

1. <span data-ttu-id="583ca-104">將 [啟用安全性預設值 **]** 切換為 [否 **]** 以停用 [Azure 安全性預設值](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="583ca-104">Disable the [Azure security defaults](/azure/active-directory/fundamentals/concept-fundamentals-security-defaults) by toggling **Enable security defaults** to **No**.</span></span>

    <span data-ttu-id="583ca-105">a.</span><span class="sxs-lookup"><span data-stu-id="583ca-105">a.</span></span> <span data-ttu-id="583ca-106">以安全性系統管理員、條件式存取系統管理員或全域系統管理員的身分登入 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="583ca-106">Sign in to the Azure portal as a Security administrator, Conditional Access administrator, or global administrator.</span></span><BR/>
    <span data-ttu-id="583ca-107">b.</span><span class="sxs-lookup"><span data-stu-id="583ca-107">b.</span></span> <span data-ttu-id="583ca-108">瀏覽至 [Azure Active Directory] > [屬性 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-108">Browse to Azure Active Directory > **Properties**.</span></span><BR/>
    <span data-ttu-id="583ca-109">c.</span><span class="sxs-lookup"><span data-stu-id="583ca-109">c.</span></span> <span data-ttu-id="583ca-110">選取 [管理安全性預設值 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-110">Select **Manage security defaults**.</span></span><BR/>
    <span data-ttu-id="583ca-111">d.</span><span class="sxs-lookup"><span data-stu-id="583ca-111">d.</span></span> <span data-ttu-id="583ca-112">將 [啟用安全性預設值 **]** 設定為 [否 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-112">Set **Enable security defaults** to **No**.</span></span><BR/>
    <span data-ttu-id="583ca-113">e.</span><span class="sxs-lookup"><span data-stu-id="583ca-113">e.</span></span> <span data-ttu-id="583ca-114">選取 [儲存 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-114">Select **Save**.</span></span>

2. <span data-ttu-id="583ca-115">在授權信箱上[啟用用戶端 SMTP 提交](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes)。</span><span class="sxs-lookup"><span data-stu-id="583ca-115">[Enable Client SMTP submission](/exchange/clients-and-mobile-in-exchange-online/authenticated-client-smtp-submission#enable-smtp-auth-for-specific-mailboxes) on the licensed mailbox.</span></span>

    <span data-ttu-id="583ca-116">a.</span><span class="sxs-lookup"><span data-stu-id="583ca-116">a.</span></span> <span data-ttu-id="583ca-117">從 Microsoft 365 系統管理中心，移至 [作用中使用者 **]**，然後選取使用者。</span><span class="sxs-lookup"><span data-stu-id="583ca-117">From the Microsoft 365 admin center, go to **Active Users**, and select the user.</span></span><BR/>
    <span data-ttu-id="583ca-118">b.</span><span class="sxs-lookup"><span data-stu-id="583ca-118">b.</span></span> <span data-ttu-id="583ca-119">前往 [郵件] 索引標籤，然後在 [電子郵件應用程式 **]** 下選取 [管理電子郵件應用程式 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-119">Go to Mail tab, and under **Email apps**, select **Manage email apps**.</span></span><BR/>
    <span data-ttu-id="583ca-120">d.</span><span class="sxs-lookup"><span data-stu-id="583ca-120">d.</span></span> <span data-ttu-id="583ca-121">確定已勾選 (已啟用) [已驗證的 SMTP **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-121">Make sure **Authenticated SMTP** is checked (enabled).</span></span><BR/>
    <span data-ttu-id="583ca-122">e.</span><span class="sxs-lookup"><span data-stu-id="583ca-122">e.</span></span> <span data-ttu-id="583ca-123">選取 [儲存變更 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-123">Select **Save changes**.</span></span><BR/>

3. <span data-ttu-id="583ca-124">在授權信箱上停用[多重要素驗證 (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa)。</span><span class="sxs-lookup"><span data-stu-id="583ca-124">[Disable Multi-Factor Authentication (MFA)](/microsoft-365/admin/security-and-compliance/set-up-multi-factor-authentication#turn-off-legacy-per-user-mfa) on the licensed mailbox.</span></span>

    <span data-ttu-id="583ca-125">a.</span><span class="sxs-lookup"><span data-stu-id="583ca-125">a.</span></span> <span data-ttu-id="583ca-126">前往 Microsoft 365 系統管理中心，然後在左側瀏覽功能表中選取 [使用者 **]**  >  [作用中使用者 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-126">Go to the Microsoft 365 admin center, and in the left navigation menu select **Users** > **Active users**.</span></span><BR/>
    <span data-ttu-id="583ca-127">b.</span><span class="sxs-lookup"><span data-stu-id="583ca-127">b.</span></span> <span data-ttu-id="583ca-128">選取 [多重要素驗證 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-128">Select **Multi-factor authentication**.</span></span><BR/>
    <span data-ttu-id="583ca-129">c.</span><span class="sxs-lookup"><span data-stu-id="583ca-129">c.</span></span> <span data-ttu-id="583ca-130">選取使用者並停用 [多重要素驗證 **]**。</span><span class="sxs-lookup"><span data-stu-id="583ca-130">Select the user and disable **Multi-Factor auth**.</span></span><BR/>
