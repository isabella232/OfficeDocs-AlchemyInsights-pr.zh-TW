---
title: 監視設定格式化的條件的存取
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 06307b57475e8828e6d4e5e01625d5100576f12b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279413"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="b4f5d-102">監視設定格式化的條件的存取</span><span class="sxs-lookup"><span data-stu-id="b4f5d-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="b4f5d-p101">針對設定格式化的條件的存取權的使用者會收到通知電子郵件不符合您的組織存取需求。若要解決，我們建議一或多個下列解決方案：</span><span class="sxs-lookup"><span data-stu-id="b4f5d-p101">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements. To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="b4f5d-p102">如果裝置假設是以註冊，通知使用者移至的公司入口網站應用程式，並確認其出現在公司入口網站。如果它不使用者應註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="b4f5d-p102">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal. If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="b4f5d-p103">在 Azure 的入口網站移至**Intune\>裝置規範**。**監視**下按一下 [**裝置規範**。檢視裝置規範報告來驗證使用者的裝置標示為相容。</span><span class="sxs-lookup"><span data-stu-id="b4f5d-p103">In the Azure portal go to **Intune \> Device compliance**. Under **Monitor** click **Device compliance**. View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="b4f5d-p104">在 Azure 的入口網站移至**Intune\>裝置規範**。在 [**管理**] 下按一下 [**原則**]。在規範遵守原則清單中，確認設定檔指派給使用者的裝置。如果沒有設定檔已指派，然後 Intune 將不能夠確認裝置的規範狀態。</span><span class="sxs-lookup"><span data-stu-id="b4f5d-p104">In the Azure portal go to **Intune \> Device compliance**. Under **Manage**, click **Policies**. In the list of compliance policies, verify that a profile is assigned to your user's device. If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="b4f5d-114">編輯使用者的設定格式化的條件存取工作分派。</span><span class="sxs-lookup"><span data-stu-id="b4f5d-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="b4f5d-115">在 Azure 的入口網站移至**Intune\>條件式存取\>原則**</span><span class="sxs-lookup"><span data-stu-id="b4f5d-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="b4f5d-116">從清單中選取的原則</span><span class="sxs-lookup"><span data-stu-id="b4f5d-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="b4f5d-117">按一下 [**使用者與群組**</span><span class="sxs-lookup"><span data-stu-id="b4f5d-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="b4f5d-p105">若要將目標放在某個人的特定原則，請將其新增至**包含**清單中。若要確保人員省略從原則，請將其新增至**排除**清單中。</span><span class="sxs-lookup"><span data-stu-id="b4f5d-p105">To target a certain policy at someone, add them to the **Include** list. To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="b4f5d-120">閱讀更多：[如何監視設定格式化的條件存取裝置](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="b4f5d-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/en-us/intune/conditional-access-exchange-monitor)</span></span>
  

