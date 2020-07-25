---
title: 應用程式保護原則
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/22/2020
ms.locfileid: "45266414"
---
# <a name="application-protection-policy"></a><span data-ttu-id="8e9d3-102">應用程式保護原則</span><span class="sxs-lookup"><span data-stu-id="8e9d3-102">Application protection policy</span></span>

<span data-ttu-id="8e9d3-103">如果您不熟悉應用程式防護原則 (APP)，請參閱[應用程式保護原則概觀](https://docs.microsoft.com/intune/apps/app-protection-policy)。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="8e9d3-104">若要開始使用 APP，請參閱[如何建立及指派應用程式保護原則](https://docs.microsoft.com/intune/app-protection-policies)。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="8e9d3-105">應用程式保護原則需求：</span><span class="sxs-lookup"><span data-stu-id="8e9d3-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="8e9d3-106">使用者擁有 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="8e9d3-107">使用者屬於應用程式保護原則鎖定的群組。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="8e9d3-108">裝置上只有一個公司使用者登入受保護的應用程式。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="8e9d3-109">應用程式已實作 [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started)。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="8e9d3-110">如需支援 SDK 的應用程式清單，請參閱 [Microsoft Intune 保護的應用程式](https://docs.microsoft.com/intune/apps-supported-intune-apps)。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="8e9d3-111">當符合上述需求的使用者登入已啟用 Intune SDK 的應用程式後，會套用原則。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="8e9d3-112">若要判斷是否已套用原則，最簡單的方法是要求使用者在原則中設定 PIN。</span><span class="sxs-lookup"><span data-stu-id="8e9d3-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="8e9d3-113">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="8e9d3-113">For more information, see:</span></span>

[<span data-ttu-id="8e9d3-114">APP/MAM 疑難排解常見問題集</span><span class="sxs-lookup"><span data-stu-id="8e9d3-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="8e9d3-115">如何驗證您的應用程式保護原則設定</span><span class="sxs-lookup"><span data-stu-id="8e9d3-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="8e9d3-116">了解應用程式保護原則傳遞時間表</span><span class="sxs-lookup"><span data-stu-id="8e9d3-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="8e9d3-117">如何監視應用程式保護原則</span><span class="sxs-lookup"><span data-stu-id="8e9d3-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)