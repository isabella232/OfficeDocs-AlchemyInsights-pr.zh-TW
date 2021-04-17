---
title: 從 AIP 移轉至合規性中心的 MIP/統一標籤
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
- "9002278"
- "5114"
ms.openlocfilehash: 12f5f5c46edd7918618c55a8a1905f3b28643092
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825362"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="427b2-102">從 AIP 移轉至合規性中心的 MIP/統一標籤</span><span class="sxs-lookup"><span data-stu-id="427b2-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="427b2-103">若要從 AIP 標籤移轉至安全性與合規性中心的統一標籤，請執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="427b2-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="427b2-104">**從 Azure 入口網站啟用保護**</span><span class="sxs-lookup"><span data-stu-id="427b2-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="427b2-105">如果您尚未這麼做，請開啟新的瀏覽器視窗，並[登入 Azure 入口網站](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)。</span><span class="sxs-lookup"><span data-stu-id="427b2-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="427b2-106">瀏覽至 [Azure 資訊保護 **]** 刀鋒視窗。</span><span class="sxs-lookup"><span data-stu-id="427b2-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="427b2-107">例如，在中樞功能表上，按一下 [所有服務 **]**，然後在 [篩選] 方塊中開始輸入 **資訊**。</span><span class="sxs-lookup"><span data-stu-id="427b2-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="427b2-108">選取 [Azure 資訊保護 **]**。</span><span class="sxs-lookup"><span data-stu-id="427b2-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="427b2-109">如果您之前未存取過 [Azure 資訊保護] 刀鋒視窗，請參閱一次性的[額外步驟](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)以將此刀鋒視窗新增至入口網站。</span><span class="sxs-lookup"><span data-stu-id="427b2-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="427b2-110">若要開啟 [Azure 資訊保護] 刀鋒視窗，您必須擁有 [Azure 資訊保護進階方案](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)或包含版權管理的 Office 365 方案。</span><span class="sxs-lookup"><span data-stu-id="427b2-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="427b2-111">如果您擁有這其中一項訂閱，但看到訊息指出找不到有效的訂閱，請[連絡 Microsoft 支援服務](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)，或使用您的標準支援通道。</span><span class="sxs-lookup"><span data-stu-id="427b2-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="427b2-112">找到 [管理 **]** 功能表選項，然後選取 [保護啟用 **]**。</span><span class="sxs-lookup"><span data-stu-id="427b2-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="427b2-113">按一下 [啟用 **]**，然後確認您的動作。</span><span class="sxs-lookup"><span data-stu-id="427b2-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="427b2-114">啟用完成時，資訊列會顯示 [已成功完成啟動 **]**。</span><span class="sxs-lookup"><span data-stu-id="427b2-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="427b2-115">**將 Azure 資訊保護標籤移轉至 Office 365 安全性與合規性中心**</span><span class="sxs-lookup"><span data-stu-id="427b2-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="427b2-116">確認您以具有全域系統管理員權限的使用者身分登入。</span><span class="sxs-lookup"><span data-stu-id="427b2-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="427b2-117">瀏覽至 [Azure 資訊保護 **]** 刀鋒視窗。</span><span class="sxs-lookup"><span data-stu-id="427b2-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="427b2-118">從 [管理 **]** 功能表選項，選取 [統一標籤 **]**。</span><span class="sxs-lookup"><span data-stu-id="427b2-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="427b2-119">在 [Azure 資訊保護 - 統一標籤 **]** 刀鋒視窗上，按一下 [啟用 **]**，並遵循線上指示進行。</span><span class="sxs-lookup"><span data-stu-id="427b2-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="427b2-120">**附註**：請先驗證您擁有適當的權限，再啟動安全性與合規性中心移轉。</span><span class="sxs-lookup"><span data-stu-id="427b2-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="427b2-121">如需詳細資訊，請參閱下列文章：</span><span class="sxs-lookup"><span data-stu-id="427b2-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="427b2-122">必須是全域系統管理員才能設定 Azure 資訊保護，或者我可以委派給其他系統管理員嗎？</span><span class="sxs-lookup"><span data-stu-id="427b2-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="427b2-123">關於移轉至安全性與合規性中心之後，系統管理角色的重要資訊。</span><span class="sxs-lookup"><span data-stu-id="427b2-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="427b2-124">如需有關 AIP 移轉至安全性與合規性中心的統一標籤的詳細資訊，請參閱[移轉標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)。</span><span class="sxs-lookup"><span data-stu-id="427b2-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
