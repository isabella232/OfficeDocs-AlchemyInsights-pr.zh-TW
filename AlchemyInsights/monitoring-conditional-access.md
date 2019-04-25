---
title: 監視的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418460"
---
# <a name="monitoring-conditional-access"></a><span data-ttu-id="3a050-102">監視的條件式存取</span><span class="sxs-lookup"><span data-stu-id="3a050-102">Monitoring Conditional Access</span></span>

<span data-ttu-id="3a050-103">使用條件式存取目標使用者會收到通知電子郵件，如果未符合您的組織存取需求。</span><span class="sxs-lookup"><span data-stu-id="3a050-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="3a050-104">若要解決，我們建議一或多個下列解決方案：</span><span class="sxs-lookup"><span data-stu-id="3a050-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="3a050-105">如果裝置會假設要註冊，通知使用者前往的公司入口網站應用程式，並確認它會出現在公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="3a050-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="3a050-106">如果沒有，則使用者應該註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="3a050-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="3a050-107">在 Azure 入口網站移至**Intune\>裝置相容性**。</span><span class="sxs-lookup"><span data-stu-id="3a050-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="3a050-108">在 [**監視**] 下按一下 [**裝置相容性**]。</span><span class="sxs-lookup"><span data-stu-id="3a050-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="3a050-109">檢視裝置合規性報告，以確認使用者的裝置標記為相容。</span><span class="sxs-lookup"><span data-stu-id="3a050-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="3a050-110">在 Azure 入口網站移至**Intune\>裝置相容性**。</span><span class="sxs-lookup"><span data-stu-id="3a050-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="3a050-111">在 [**管理**] 下按一下 [**原則**]。</span><span class="sxs-lookup"><span data-stu-id="3a050-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="3a050-112">在符合性原則清單中，確認設定檔指派給使用者的裝置。</span><span class="sxs-lookup"><span data-stu-id="3a050-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="3a050-113">如果沒有設定檔指派，然後 Intune 將無法確認裝置的合規性狀態。</span><span class="sxs-lookup"><span data-stu-id="3a050-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="3a050-114">編輯使用者的條件式存取工作分派。</span><span class="sxs-lookup"><span data-stu-id="3a050-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="3a050-115">在 Azure 入口網站移至 [ **Intune\>條件式存取\>原則**</span><span class="sxs-lookup"><span data-stu-id="3a050-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="3a050-116">從清單中選取原則</span><span class="sxs-lookup"><span data-stu-id="3a050-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="3a050-117">按一下 [**使用者和群組**</span><span class="sxs-lookup"><span data-stu-id="3a050-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="3a050-118">若要為目標的特定原則的人員，請將其新增至 [**包含**清單中。</span><span class="sxs-lookup"><span data-stu-id="3a050-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="3a050-119">若要確保人員省略從原則，請將其新增至**排除**清單中。</span><span class="sxs-lookup"><span data-stu-id="3a050-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="3a050-120">閱讀其他資訊：[如何監視條件式存取裝置](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="3a050-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

