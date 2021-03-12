---
title: 監視條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708665"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="1982a-102">監視 Exchange 的條件式存取</span><span class="sxs-lookup"><span data-stu-id="1982a-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="1982a-103">以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。</span><span class="sxs-lookup"><span data-stu-id="1982a-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="1982a-104">若要解決此問題，我們建議下列一或多個解決方案：</span><span class="sxs-lookup"><span data-stu-id="1982a-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="1982a-105">若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="1982a-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="1982a-106">如果不是，則使用者應該註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="1982a-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="1982a-107">在 Azure 入口網站中，移至 Intune > 裝置規範。</span><span class="sxs-lookup"><span data-stu-id="1982a-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="1982a-108">在 [監視器] 底下按一下 [裝置符合性]。</span><span class="sxs-lookup"><span data-stu-id="1982a-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="1982a-109">查看您的裝置符合性報告，以確認使用者的裝置已標示為相容。</span><span class="sxs-lookup"><span data-stu-id="1982a-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="1982a-110">在 Azure 入口網站中，移至 Intune > 裝置規範。</span><span class="sxs-lookup"><span data-stu-id="1982a-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="1982a-111">在 [管理] 下，按一下 [原則]。</span><span class="sxs-lookup"><span data-stu-id="1982a-111">Under Manage, click Policies.</span></span> <span data-ttu-id="1982a-112">在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。</span><span class="sxs-lookup"><span data-stu-id="1982a-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="1982a-113">若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。</span><span class="sxs-lookup"><span data-stu-id="1982a-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="1982a-114">編輯使用者的條件式存取指派。</span><span class="sxs-lookup"><span data-stu-id="1982a-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="1982a-115">在 Azure 入口網站中，移至 **Intune**  >  **條件式存取**  >  **原則**。</span><span class="sxs-lookup"><span data-stu-id="1982a-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="1982a-116">從清單中選取原則。</span><span class="sxs-lookup"><span data-stu-id="1982a-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="1982a-117">按一下 [使用者和群組]。</span><span class="sxs-lookup"><span data-stu-id="1982a-117">Click Users and groups.</span></span>
4. <span data-ttu-id="1982a-118">若要以某人為目標設定特定原則，請將其新增至 [包含] 清單。</span><span class="sxs-lookup"><span data-stu-id="1982a-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="1982a-119">若要確保從原則中省略了某個人員，請將其新增至 [排除] 清單。</span><span class="sxs-lookup"><span data-stu-id="1982a-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="1982a-120">有用的連結：</span><span class="sxs-lookup"><span data-stu-id="1982a-120">Helpful links:</span></span>

[<span data-ttu-id="1982a-121">裝置合規性概述</span><span class="sxs-lookup"><span data-stu-id="1982a-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="1982a-122">疑難排解 CA</span><span class="sxs-lookup"><span data-stu-id="1982a-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="1982a-123">疑難排解原則</span><span class="sxs-lookup"><span data-stu-id="1982a-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="1982a-124">監控 Intune 裝置合規性</span><span class="sxs-lookup"><span data-stu-id="1982a-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="1982a-125">附注：這些步驟僅有助於疑難排解 Azure Active Directory 功能條件式存取。</span><span class="sxs-lookup"><span data-stu-id="1982a-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="1982a-126">您也可以隔離透過 Exchange 原則封鎖它的電子郵件存取的裝置。</span><span class="sxs-lookup"><span data-stu-id="1982a-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="1982a-127">您可以在 [這裡] 找到 Exchange 裝置管理的詳細資訊 [這裡] (https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) 。</span><span class="sxs-lookup"><span data-stu-id="1982a-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
