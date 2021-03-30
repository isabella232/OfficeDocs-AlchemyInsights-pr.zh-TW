---
title: 驗證應用程式
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403801"
---
# <a name="authentication-app"></a><span data-ttu-id="e9357-102">驗證應用程式</span><span class="sxs-lookup"><span data-stu-id="e9357-102">Authentication app</span></span>

<span data-ttu-id="e9357-103">如果您是全域系統管理員，您可以使用登 [入診斷](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)，快速找出與使用者登入相關的問題。</span><span class="sxs-lookup"><span data-stu-id="e9357-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="e9357-104">按一下 [[啟動診斷](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)] 按鈕，啟動診斷程式。</span><span class="sxs-lookup"><span data-stu-id="e9357-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="e9357-105">輸入您所擁有的使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼的詳細資料，以尋找要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="e9357-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="e9357-106">檢閱診斷結果 - 顯示有關所發生的事件以及可採取哪些動作以進行變更的詳細資料 (如果需要變更的話)。</span><span class="sxs-lookup"><span data-stu-id="e9357-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="e9357-107">**檢查適用的案例：**</span><span class="sxs-lookup"><span data-stu-id="e9357-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="e9357-108">如果使用者未在 Microsoft 驗證器應用程式中取得推播通知，請確認在 [MFA 封鎖] 使用者未如 [封鎖和解除封鎖使用者](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)中所述的那樣顯示這些使用者。</span><span class="sxs-lookup"><span data-stu-id="e9357-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="e9357-109">如果使用者未被封鎖進行 MFA，但沒有收到推播通知，則可以開啟 Microsoft 驗證者應用程式，它會拉出擱置的核准要求。</span><span class="sxs-lookup"><span data-stu-id="e9357-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="e9357-110">另一種登入方法，使用者也可以按一下登入另一種方式，然後選擇 [使用我的行動應用程式的驗證碼。</span><span class="sxs-lookup"><span data-stu-id="e9357-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="e9357-111">Microsoft 驗證應用程式是許多使用者唯一可用的方法。</span><span class="sxs-lookup"><span data-stu-id="e9357-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="e9357-112">[深入瞭解安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)，請參閱 [驗證器 App 應用程式](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) 常見問題，以取得常見問題及其解決方法。</span><span class="sxs-lookup"><span data-stu-id="e9357-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="e9357-113">**建議影片**</span><span class="sxs-lookup"><span data-stu-id="e9357-113">**Recommended Videos**</span></span>

<span data-ttu-id="e9357-114">[如何在新電話上設定驗證器應用程式 (2min) ](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)。</span><span class="sxs-lookup"><span data-stu-id="e9357-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
