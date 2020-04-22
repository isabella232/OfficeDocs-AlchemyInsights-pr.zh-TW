---
title: 監視條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713709"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="d7957-102">監視 Exchange 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="d7957-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="d7957-103">以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。</span><span class="sxs-lookup"><span data-stu-id="d7957-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="d7957-104">若要解決此問題，我們建議下列一或多個解決方案：</span><span class="sxs-lookup"><span data-stu-id="d7957-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="d7957-105">若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="d7957-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="d7957-106">如果不是，則使用者應該註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="d7957-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="d7957-107">在 Azure 入口網站中，移至\*\* \> Intune 裝置規範\*\*。</span><span class="sxs-lookup"><span data-stu-id="d7957-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="d7957-108">在 [**監視器**] 底下按一下 [**裝置符合性**]。</span><span class="sxs-lookup"><span data-stu-id="d7957-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="d7957-109">查看您的裝置符合性報告，以確認使用者的裝置已標示為相容。</span><span class="sxs-lookup"><span data-stu-id="d7957-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="d7957-110">在 Azure 入口網站中，移至\*\* \> Intune 裝置規範\*\*。</span><span class="sxs-lookup"><span data-stu-id="d7957-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="d7957-111">在 [**管理**] 下，按一下 [**原則**]。</span><span class="sxs-lookup"><span data-stu-id="d7957-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="d7957-112">在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。</span><span class="sxs-lookup"><span data-stu-id="d7957-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="d7957-113">若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。</span><span class="sxs-lookup"><span data-stu-id="d7957-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="d7957-114">編輯使用者的條件式存取指派。</span><span class="sxs-lookup"><span data-stu-id="d7957-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="d7957-115">在 Azure 入口網站移至**Intune \>條件式\>存取原則**</span><span class="sxs-lookup"><span data-stu-id="d7957-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="d7957-116">從清單中選取原則</span><span class="sxs-lookup"><span data-stu-id="d7957-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="d7957-117">按一下 [**使用者和群組**]</span><span class="sxs-lookup"><span data-stu-id="d7957-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="d7957-118">若要以某人為目標設定特定原則，請將其新增至 [**包含**] 清單。</span><span class="sxs-lookup"><span data-stu-id="d7957-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="d7957-119">若要確保從原則中省略了某個人員，請將其新增至 [**排除**] 清單。</span><span class="sxs-lookup"><span data-stu-id="d7957-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="d7957-120">閱讀其他資訊：[如何監視條件式存取裝置](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="d7957-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

