---
title: 我受到符合規範裝置的條件式存取封鎖
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897676"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a><span data-ttu-id="7f4a5-102">我受到符合規範裝置的條件式存取封鎖</span><span class="sxs-lookup"><span data-stu-id="7f4a5-102">I’m getting blocked by Conditional Access with compliant device</span></span>

<span data-ttu-id="7f4a5-103">**強烈建議的工具**</span><span class="sxs-lookup"><span data-stu-id="7f4a5-103">**Highly Recommended Tools**</span></span>

- <span data-ttu-id="7f4a5-104">[裝置註冊疑難排解員工具](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 完整的工具，可協助疑難排解最常見的裝置註冊問題。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-104">[Device Registration Troubleshooter Tool](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - A comprehensive tool that helps troubleshoot the most common device registration issues.</span></span>
- <span data-ttu-id="7f4a5-105">[測試裝置註冊連線能力指令碼](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - 用來確保裝置可以存取系統帳戶下裝置註冊端點的工具。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-105">[Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - A tool used to ensure that a device can access Device Registration endpoints under the system account.</span></span>
- <span data-ttu-id="7f4a5-106">[Azure AD 裝置清理指令碼](https://github.com/mzmaili/AzureADDeviceCleanup) - 用來尋找和管理您環境中過時裝置的工具。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-106">[Azure AD Device Cleanup Script](https://github.com/mzmaili/AzureADDeviceCleanup) - A tool used to seek and manage stale devices in your environment.</span></span>

<span data-ttu-id="7f4a5-107">以下是條件式存取在符合規範的裝置上可能會失敗的原因，或為何在組織資源的登入要求期間，您的使用者可能會收到 **[您無法從這裡完成]** 的訊息。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-107">Here are some common reasons why Conditional Access may be failing for a compliant device or why your users may be receiving **You can't get there from here** message during a sign-in request to an organizational resource.</span></span>

1. <span data-ttu-id="7f4a5-108">**裝置不是使用 MDM 所需的裝置狀態**：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-108">**Device is not in a required device state with an MDM**:</span></span>

<span data-ttu-id="7f4a5-109">驗證裝置是否向核准的 MDM 提供者 (例如 Intune) 註冊，並 *標示為符合規範*。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-109">Validate that the device is enrolled with an approved MDM provider like Intune and *marked as compliant*.</span></span> <span data-ttu-id="7f4a5-110">如需有關 Intune 的詳細資訊，請參閱本[文件](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-110">For more information on Intune see this [document](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment).</span></span> <span data-ttu-id="7f4a5-111">若要深入瞭解裝置合規性和 Intune，請參閱[使用合規性原則為使用 Intune 管理的裝置設定規則](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-111">For better understanding of device compliance and Intune, see [use compliance policy to set rules for devices you manage with Intune](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started).</span></span> <span data-ttu-id="7f4a5-112">如果您在使用 Intune 註冊裝置時遇到問題，請參閱 [在 Microsoft 中對裝置註冊進行疑難排解](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) (部分機器翻譯) 上的疑難排解詳細資料。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-112">If you are having issues enrolling a device with Intune, find troubleshooting details at [Troubleshoot device enrollment in Microsoft](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span> <span data-ttu-id="7f4a5-113">若要進一步獲得 Intune 支援，請建立支援要求。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-113">For further Intune support, create a support request.</span></span> <span data-ttu-id="7f4a5-114">若要這樣做，請瀏覽 [Intune 的協助及支援頁面](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-114">To do so, visit the [Intune Help and Support page](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport).</span></span>

2. <span data-ttu-id="7f4a5-115">**裝置未加入組織網路**：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-115">**Device is not joined to the organizations network**:</span></span>

<span data-ttu-id="7f4a5-116">若要存取組織資源，裝置必須透過直接連線或虛擬私人網路 (VPN) 連線到組織的網路，並且也加入內部部署或 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-116">For access to organizational resources, the device has to be connected to the organization's network, either through direct connection or a virtual private network (VPN), and also joined to on-premise or Azure Active Directory.</span></span> <span data-ttu-id="7f4a5-117">若要將工作裝置加入組織網路，請參閱[將您的工作裝置加入組織的網路](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-117">To join a work device to the organization network, see [Join your work device to your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network).</span></span> <span data-ttu-id="7f4a5-118">若要註冊個人/BYOD 裝置，請參閱[在組織的網路上註冊您的個人裝置](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-118">To register a personal/BYOD device, see [Register your personal device on your organization's network](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network).</span></span>

- <span data-ttu-id="7f4a5-119">若要驗證裝置是否已加入網路，您可以按照[此處](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) (部分機器翻譯) 的步驟註冊裝置，或[此處](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined) (部分機器翻譯) 的步驟註冊工作裝置。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-119">To validate whether the device has joined the network, you can follow the steps for registered devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered) or work devices [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined).</span></span> <span data-ttu-id="7f4a5-120">若要將問題的範圍縮小為組織網路連線，請遵循下列指導方針：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-120">To scope the issue to Org network connectivity, follow guidelines below:</span></span>

    1. <span data-ttu-id="7f4a5-121">使用工作或學校帳戶登入 Windows，例如 alain@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-121">Sign in to Windows using your work or school account,  for example, alain@contoso.com.</span></span>
    2. <span data-ttu-id="7f4a5-122">透過 VPN 或 DirectAccess 連線到貴組織的網路。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-122">Connect to your organization's network through a VPN or DirectAccess.</span></span>
    3. <span data-ttu-id="7f4a5-123">連線之後，請按 **Windows 標誌鍵+L** 鎖定您的裝置。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-123">After you're connected, press the **Windows logo key+L** to lock your device.</span></span>
    4. <span data-ttu-id="7f4a5-124">使用公司或學校帳戶解除鎖定您的裝置，然後再次嘗試存取有問題的應用程式或服務。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-124">Unlock your device using your work or school account, and then try to access the problematic app or service again.</span></span>

<span data-ttu-id="7f4a5-125">如果您再次看到 **[您無法從這裡完成]** 錯誤訊息，問題可能出在其他地方。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-125">If you see the **You can't get there from here** error message again, issue is likely elsewhere.</span></span>

3. <span data-ttu-id="7f4a5-126">**不支援的作業系統**：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-126">**Operating system is not supported**:</span></span>

<span data-ttu-id="7f4a5-127">請確保您目前的作業系統版本受支援，包括：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-127">Ensure that you're running a supported version of the operating system, including:</span></span>

- <span data-ttu-id="7f4a5-128">**Windows 用戶端**：Windows 7 或更新版本</span><span class="sxs-lookup"><span data-stu-id="7f4a5-128">**Windows Client**: Windows 7 or later</span></span>

- <span data-ttu-id="7f4a5-129">**Windows 伺服器**：Windows Server 2008 R2 或更新版本</span><span class="sxs-lookup"><span data-stu-id="7f4a5-129">**Windows Server**: Windows Server 2008 R2 or later</span></span>

- <span data-ttu-id="7f4a5-130">**macOS**：macOS X 或更新版本</span><span class="sxs-lookup"><span data-stu-id="7f4a5-130">**macOS**: macOS X or later</span></span>

- <span data-ttu-id="7f4a5-131">**Android 和 iOS**：最新版本的 Android 和 iOS 行動裝置作業系統</span><span class="sxs-lookup"><span data-stu-id="7f4a5-131">**Android and iOS**: Latest version of Android and iOS mobile operating systems</span></span>

4. <span data-ttu-id="7f4a5-132">**不支援的網頁瀏覽器**：</span><span class="sxs-lookup"><span data-stu-id="7f4a5-132">**Web browser is not supported**:</span></span>

<span data-ttu-id="7f4a5-133">請在下方尋找支援的瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-133">Please find supported browsers below.</span></span> <span data-ttu-id="7f4a5-134">對於 Windows 1703 或更新版本的 Chrome 支援，需要 Windows 10 帳戶擴充功能。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-134">For Chrome support with Windows 1703 or later versions, a Windows 10 Accounts extension is required.</span></span> <span data-ttu-id="7f4a5-135">對於 Microsoft Edge 85+，使用者必須登入，以正確傳遞裝置合規性資訊。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-135">For Edge 85+, the user needs to be signed in to properly pass device compliance information.</span></span> <span data-ttu-id="7f4a5-136">如需詳細資訊，請參閱[此處](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-136">For more details, see [here](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support).</span></span>

- <span data-ttu-id="7f4a5-137">**Windows 10**：Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="7f4a5-137">**Windows 10**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="7f4a5-138">**Windows 8 / 8.1**：Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="7f4a5-138">**Windows 8 / 8.1**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="7f4a5-139">**Windows 7**：Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="7f4a5-139">**Windows 7**: Internet Explorer, Chrome</span></span>
- <span data-ttu-id="7f4a5-140">**iOS**：Microsoft Edge、Intune Managed Browser、Safari</span><span class="sxs-lookup"><span data-stu-id="7f4a5-140">**iOS**: Microsoft Edge, Intune Managed Browser, Safari</span></span>
- <span data-ttu-id="7f4a5-141">**Android**：**Microsoft Edge**：Intune Managed Browser、Chrome</span><span class="sxs-lookup"><span data-stu-id="7f4a5-141">**Android**: **Microsoft Edge**: Intune Managed Browser, Chrome</span></span>
- <span data-ttu-id="7f4a5-142">**Windows Phone**：Microsoft Edge、Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="7f4a5-142">**Windows Phone**: Microsoft Edge, Internet Explorer</span></span>
- <span data-ttu-id="7f4a5-143">**Windows Server 2019**：Microsoft Edge、Internet Explorer、Chrome</span><span class="sxs-lookup"><span data-stu-id="7f4a5-143">**Windows Server 2019**: Microsoft Edge, Internet Explorer, Chrome</span></span>
- <span data-ttu-id="7f4a5-144">**Windows Server 2016**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="7f4a5-144">**Windows Server 2016**: Internet Explorer</span></span>
- <span data-ttu-id="7f4a5-145">**Windows Server 2012 R2**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="7f4a5-145">**Windows Server 2012 R2**: Internet Explorer</span></span>
- <span data-ttu-id="7f4a5-146">**Windows Server 2008 R2**：Internet Explorer</span><span class="sxs-lookup"><span data-stu-id="7f4a5-146">**Windows Server 2008 R2**: Internet Explorer</span></span>
- <span data-ttu-id="7f4a5-147">**macOS**：Chrome、Safari</span><span class="sxs-lookup"><span data-stu-id="7f4a5-147">**macOS**: Chrome, Safari</span></span>

<span data-ttu-id="7f4a5-148">在 [這裡](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation) (部分機器翻譯) 找到有關 **[您無法從這裡完成]** 的訊息和疑難排解步驟。</span><span class="sxs-lookup"><span data-stu-id="7f4a5-148">Find more information on the **You can't get there** message and troubleshooting steps [here](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation).</span></span>
