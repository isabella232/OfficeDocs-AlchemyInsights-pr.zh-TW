---
title: 疑難排解問題註冊 Microsoft Intune 中的 Android 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 1e1d50c31df588a3416d758d40fbd7bde3f73b21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500062"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="52379-102">疑難排解問題註冊 Microsoft Intune 中的 Android 裝置</span><span class="sxs-lookup"><span data-stu-id="52379-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="52379-103">請先檢閱下列資源以立即解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="52379-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="52379-104">部分一般問題及解決步驟：</span><span class="sxs-lookup"><span data-stu-id="52379-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="52379-105">**裝置未加密的公司入口網站中的錯誤：** 較新版本的 Android，尤其開頭 v7.0，需要啟動密碼以確保您的裝置已完全加密。</span><span class="sxs-lookup"><span data-stu-id="52379-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="52379-106">若要啟用啟動 pin 碼，或完全加密裝置是常見的解決方案。</span><span class="sxs-lookup"><span data-stu-id="52379-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="52379-107">檢閱[本文件](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="52379-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="52379-108">**裝置無法簽入 Intune 服務或 Intune 管理主控台中顯示為 「 Unhealthy 」:** 某些 Samsung 4.4 和 5.5 裝置可能會檢查恢復服務。</span><span class="sxs-lookup"><span data-stu-id="52379-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="52379-109">有 3 可能的解決方案，此問題：</span><span class="sxs-lookup"><span data-stu-id="52379-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="52379-110">以手動方式開啟 Intune 公司入口網站應用程式，將會自動啟動裝置同步處理。</span><span class="sxs-lookup"><span data-stu-id="52379-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="52379-111">更新裝置 Android 6.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="52379-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="52379-112">停用 Samsung 智慧管理員從管理 Intune 公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="52379-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="52379-113">檢閱[本文件](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)如需這些問題與解決方法的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="52379-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="52379-114">**使用者授權類型不正確**或**使用者名稱無法辨識的錯誤：** 使用者需要已獲得 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="52379-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="52379-115">檢閱這些文件以透過將授權指派： Office 系統管理中心或 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="52379-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="52379-116">其他資源，可以協助解決您的問題：</span><span class="sxs-lookup"><span data-stu-id="52379-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="52379-117">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="52379-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="52379-118">檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="52379-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="52379-119">檢閱[本文件](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的清單中的每個防止註冊和解決方法的常見錯誤。</span><span class="sxs-lookup"><span data-stu-id="52379-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="52379-120">[了解如何註冊 Microsoft Intune 中的 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="52379-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
