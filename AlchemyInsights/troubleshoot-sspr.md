---
title: 疑難排解 SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428692"
---
# <a name="troubleshoot-sspr"></a><span data-ttu-id="c30cf-102">疑難排解 SSPR</span><span class="sxs-lookup"><span data-stu-id="c30cf-102">Troubleshoot SSPR</span></span>

<span data-ttu-id="c30cf-103">**設定密碼重設時有問題**</span><span class="sxs-lookup"><span data-stu-id="c30cf-103">**I'm having trouble configuring password reset**</span></span>

- <span data-ttu-id="c30cf-104">如果您是系統管理員，並尋找如何啟用自助密碼重設，請參閱 [教學課程啟用 SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)，為您的組織設定密碼重設。</span><span class="sxs-lookup"><span data-stu-id="c30cf-104">If you are administrator and looking for how to enable self-service password reset, see [Tutorial enable SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), to configure password reset for your organization.</span></span> <span data-ttu-id="c30cf-105">您也可能想要複查 [授權要求](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="c30cf-105">You may also want to review the [licensing requirements](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span> <span data-ttu-id="c30cf-106">您的組織中必須至少有一個指派的授權。</span><span class="sxs-lookup"><span data-stu-id="c30cf-106">You must have at least one license assigned in your organization.</span></span>
    - <span data-ttu-id="c30cf-107">**僅限雲端使用者** -任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="c30cf-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="c30cf-108">**雲端和/或內部部署使用者** -Azure AD Premium P1 或 P2、Enterprise 可移動性 + SECURITY (EMS) 或安全生產力 (SPE) </span><span class="sxs-lookup"><span data-stu-id="c30cf-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
- <span data-ttu-id="c30cf-109">如需有關自助密碼重設的其他問題，請參閱 [我們的常見問題解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="c30cf-109">For additional questions about self-service password reset, review [our FAQ](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="c30cf-110">**我收到錯誤訊息**</span><span class="sxs-lookup"><span data-stu-id="c30cf-110">**I'm getting an error message**</span></span>

<span data-ttu-id="c30cf-111">請參閱本文以尋找常見的錯誤及其解決方法： [自助密碼重設疑難排解](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="c30cf-111">Review this article to find common errors and their solutions: [Troubleshoot self-service password reset](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="c30cf-112">**密碼重設原則發生問題**</span><span class="sxs-lookup"><span data-stu-id="c30cf-112">**I'm having a problem with my password reset policy**</span></span>

- <span data-ttu-id="c30cf-113">如果您的密碼重設原則行為意外，或是您有有關密碼重設原則的問題，請參閱下列文章： [Azure Active Directory 中的密碼原則和限制](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)。</span><span class="sxs-lookup"><span data-stu-id="c30cf-113">If your password reset policy is not behaving as expected, or if you have questions about password reset policies, review this article: [Password policies and restrictions in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="c30cf-114">密碼重設原則不適用於管理員。</span><span class="sxs-lookup"><span data-stu-id="c30cf-114">Password reset policies do not apply to administrators.</span></span> <span data-ttu-id="c30cf-115">Microsoft 對任何 Azure 系統管理員角色強制實施強預設雙門密碼重設原則。</span><span class="sxs-lookup"><span data-stu-id="c30cf-115">Microsoft enforces a strong default two-gate password reset policy for any Azure administrator role.</span></span> <span data-ttu-id="c30cf-116">確定您正在使用非系統管理員的使用者進行測試。</span><span class="sxs-lookup"><span data-stu-id="c30cf-116">Make sure that you are testing with a user who is not an administrator.</span></span> <span data-ttu-id="c30cf-117">如需系統管理員重設原則的詳細資訊，請參閱下列文章： [系統管理員重設原則差異](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)。</span><span class="sxs-lookup"><span data-stu-id="c30cf-117">For more information on the administrator reset policy, see this article: [Administrator reset policy differences](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).</span></span>

<span data-ttu-id="c30cf-118">**我不想要讓使用者註冊其他安全性資訊以進行密碼重設**</span><span class="sxs-lookup"><span data-stu-id="c30cf-118">**I don't want my users to register additional security info for password reset**</span></span>

<span data-ttu-id="c30cf-119">您可以使用 API、PowerShell 或 Azure AD Connect，預先填入 (電子郵件和電話屬性) 使用者的資料。</span><span class="sxs-lookup"><span data-stu-id="c30cf-119">You can pre-populate data (email and phone attributes) for your users using an API, PowerShell, or Azure AD Connect.</span></span> <span data-ttu-id="c30cf-120">若要深入瞭解，請參閱：</span><span class="sxs-lookup"><span data-stu-id="c30cf-120">To learn how read:</span></span>

- [<span data-ttu-id="c30cf-121">部署密碼重設，但不需要使用者註冊</span><span class="sxs-lookup"><span data-stu-id="c30cf-121">Deploying password reset without requiring users to register</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [<span data-ttu-id="c30cf-122">密碼重設所使用的資料</span><span class="sxs-lookup"><span data-stu-id="c30cf-122">What data is used by password reset</span></span>](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="c30cf-123">**我想要讓使用者註冊其其他安全性資訊以進行密碼重設**</span><span class="sxs-lookup"><span data-stu-id="c30cf-123">**I want my users to register their additional security info for password reset**</span></span>

1. <span data-ttu-id="c30cf-124">讓您的使用者向 [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info)註冊自助服務密碼重設的安全性資訊。</span><span class="sxs-lookup"><span data-stu-id="c30cf-124">Have your users register their security info for self service password reset by directing them to [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info).</span></span>
1. <span data-ttu-id="c30cf-125">在使用者或由系統管理員) 為使用者 (填入資料後，請指引使用者 [aka.ms/sspr](https://passwordreset.microsoftonline.com/) ，讓使用者可以自行重設自己的密碼。</span><span class="sxs-lookup"><span data-stu-id="c30cf-125">After data is populated for the user (by the user or by the admin), direct your user to [aka.ms/sspr](https://passwordreset.microsoftonline.com/) so your users can be empowered to reset their own passwords.</span></span>
1. <span data-ttu-id="c30cf-126">如果使用者仍遇到問題，表示他們 **最可能是** 同盟或 **密碼雜湊同步** 使用者。</span><span class="sxs-lookup"><span data-stu-id="c30cf-126">If users are still experiencing problems they are most likely **federated** or **password hash synched** users.</span></span> <span data-ttu-id="c30cf-127">這表示密碼寫回服務可能發生問題。</span><span class="sxs-lookup"><span data-stu-id="c30cf-127">This means there is likely a problem with the Password Writeback service.</span></span>