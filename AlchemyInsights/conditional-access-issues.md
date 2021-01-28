---
title: 條件式存取問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013928"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="8a895-102">條件式存取問題</span><span class="sxs-lookup"><span data-stu-id="8a895-102">Conditional access issues</span></span>

<span data-ttu-id="8a895-103">**解決登入診斷的問題**</span><span class="sxs-lookup"><span data-stu-id="8a895-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="8a895-104">您可以使用登 [入診斷](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)，快速找出或診斷使用者登入相關問題：</span><span class="sxs-lookup"><span data-stu-id="8a895-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="8a895-105">啟動 登入診斷。</span><span class="sxs-lookup"><span data-stu-id="8a895-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="8a895-106">輸入您所擁有的使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼的詳細資料，以尋找要分析的事件。</span><span class="sxs-lookup"><span data-stu-id="8a895-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="8a895-107">查看診斷結果，顯示發生什麼情況的詳細資料，以及您可以採取哪些動作進行變更 (若) 需要任何變更。</span><span class="sxs-lookup"><span data-stu-id="8a895-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="8a895-108">**疑難排解 Sign-In 的步驟**</span><span class="sxs-lookup"><span data-stu-id="8a895-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="8a895-109">流覽至 Azure AD 登入頁面。</span><span class="sxs-lookup"><span data-stu-id="8a895-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="8a895-110">篩選登入的使用者、時間範圍、應用程式、狀態、用戶端應用程式等等。</span><span class="sxs-lookup"><span data-stu-id="8a895-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="8a895-111">選取登入事件，然後查看 [條件存取] 索引標籤，以查看已評估的原則。</span><span class="sxs-lookup"><span data-stu-id="8a895-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="8a895-112">按一下原則的列，以查看原則詳細資料並瞭解其應用原因。</span><span class="sxs-lookup"><span data-stu-id="8a895-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="8a895-113">**設定條件式存取原則疑難排解的工具**</span><span class="sxs-lookup"><span data-stu-id="8a895-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="8a895-114">僅限報告模式可讓您評估原則，而不會影響使用者。</span><span class="sxs-lookup"><span data-stu-id="8a895-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="8a895-115">假設工具可讓您模擬登入事件，並查看適用的原則。</span><span class="sxs-lookup"><span data-stu-id="8a895-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="8a895-116">Insights 與報告活頁簿會顯示每個原則的即時影響。</span><span class="sxs-lookup"><span data-stu-id="8a895-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="8a895-117">**基準保護原則**</span><span class="sxs-lookup"><span data-stu-id="8a895-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="8a895-118">已棄用基準保護原則。</span><span class="sxs-lookup"><span data-stu-id="8a895-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="8a895-119">它們不再執行，很快就會從 Azure 入口網站移除。</span><span class="sxs-lookup"><span data-stu-id="8a895-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="8a895-120">建議啟用 [安全性預設值](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)。</span><span class="sxs-lookup"><span data-stu-id="8a895-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="8a895-121">如需條件式存取的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="8a895-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="8a895-122">[在 Azure Active Directory 中進行條件式存取的最佳作法](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
[條件式存取](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 中的條件[條件式存取](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 中的控制項[條件式存取中的位置](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="8a895-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
