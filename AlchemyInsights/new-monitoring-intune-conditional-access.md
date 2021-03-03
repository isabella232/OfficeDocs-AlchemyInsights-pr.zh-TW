---
title: 監視 Intune 條件式存取
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "50417110"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="512ef-102">監視 Intune 條件式存取</span><span class="sxs-lookup"><span data-stu-id="512ef-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="512ef-103">以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。</span><span class="sxs-lookup"><span data-stu-id="512ef-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="512ef-104">若要解決此問題，我們建議下列一或多個解決方案：</span><span class="sxs-lookup"><span data-stu-id="512ef-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="512ef-105">若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="512ef-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="512ef-106">如果不是，則使用者必須註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="512ef-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="512ef-107">在 Azure 入口網站中，移至 **Intune**  >  **裝置規範**。</span><span class="sxs-lookup"><span data-stu-id="512ef-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="512ef-108">若要查看您的裝置符合性報告，以確認使用者的裝置標示為相容，請按一下 [ **監視器**] 底下的 [ **裝置符合性**]。</span><span class="sxs-lookup"><span data-stu-id="512ef-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="512ef-109">在 Azure 入口網站中，移至 **Intune**  >  **裝置規範**。</span><span class="sxs-lookup"><span data-stu-id="512ef-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="512ef-110">在 [管理] 下 **，** 按一下 [ **原則**]。</span><span class="sxs-lookup"><span data-stu-id="512ef-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="512ef-111">在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。</span><span class="sxs-lookup"><span data-stu-id="512ef-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="512ef-112">若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。</span><span class="sxs-lookup"><span data-stu-id="512ef-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="512ef-113">編輯使用者的條件式存取指派。</span><span class="sxs-lookup"><span data-stu-id="512ef-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="512ef-114">在 Azure 入口網站中，流覽至 [ **Intune**  >  **條件式存取**  >  **原則**]，從清單中選取原則，然後按一下 [**使用者和群組**]。</span><span class="sxs-lookup"><span data-stu-id="512ef-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="512ef-115">若要以某人為目標設定特定原則，請將其新增至 [ **包含] 清單**。</span><span class="sxs-lookup"><span data-stu-id="512ef-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="512ef-116">若要確保從原則中省略了某個人員，請將其新增至 [ **排除] 清單**。</span><span class="sxs-lookup"><span data-stu-id="512ef-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="512ef-117">**有用的連結：**</span><span class="sxs-lookup"><span data-stu-id="512ef-117">**Helpful links:**</span></span>

- [<span data-ttu-id="512ef-118">裝置合規性概述</span><span class="sxs-lookup"><span data-stu-id="512ef-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="512ef-119">疑難排解 CA</span><span class="sxs-lookup"><span data-stu-id="512ef-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="512ef-120">疑難排解原則</span><span class="sxs-lookup"><span data-stu-id="512ef-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="512ef-121">監控 Intune 裝置合規性</span><span class="sxs-lookup"><span data-stu-id="512ef-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="512ef-122">這些步驟只有助于疑難排解 Azure Active Directory 功能條件式存取。</span><span class="sxs-lookup"><span data-stu-id="512ef-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="512ef-123">您也可以隔離透過 Exchange 原則封鎖它的電子郵件存取的裝置。</span><span class="sxs-lookup"><span data-stu-id="512ef-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="512ef-124">您可以在 [**這裡**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))找到 Exchange 裝置管理的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="512ef-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
