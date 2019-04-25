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
ms.openlocfilehash: 0e727bd47a7d549a439e4666fa9dbb8a02e39778
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420583"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="60405-102">疑難排解問題註冊 Microsoft Intune 中的 Android 裝置</span><span class="sxs-lookup"><span data-stu-id="60405-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="60405-103">請先檢閱下列資源以立即解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="60405-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="60405-104">部分一般問題及解決步驟：</span><span class="sxs-lookup"><span data-stu-id="60405-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="60405-105">**裝置未加密的公司入口網站中的錯誤：** 較新版本的 Android，尤其開頭 v7.0，需要啟動密碼以確保您的裝置已完全加密。</span><span class="sxs-lookup"><span data-stu-id="60405-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="60405-106">若要啟用啟動 pin 碼，或完全加密裝置是常見的解決方案。</span><span class="sxs-lookup"><span data-stu-id="60405-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="60405-107">檢閱[本文件](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="60405-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="60405-108">**裝置無法簽入 Intune 服務或 Intune 管理主控台中顯示為 「 Unhealthy 」:** 某些 Samsung 4.4 和 5.5 裝置可能會檢查恢復服務。</span><span class="sxs-lookup"><span data-stu-id="60405-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="60405-109">有 3 可能的解決方案，此問題：</span><span class="sxs-lookup"><span data-stu-id="60405-109">There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="60405-110">以手動方式開啟 Intune 公司入口網站應用程式，將會自動啟動裝置同步處理。</span><span class="sxs-lookup"><span data-stu-id="60405-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="60405-111">更新裝置 Android 6.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="60405-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="60405-112">停用 Samsung 智慧管理員從管理 Intune 公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="60405-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="60405-113">檢閱[本文件](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)如需這些問題與解決方法的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="60405-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="60405-114">**使用者授權類型不正確**或**使用者名稱無法辨識的錯誤：** 使用者需要已獲得 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="60405-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="60405-115">檢閱這些文件以透過將授權指派： Office 系統管理中心或 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="60405-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="60405-116">其他資源，可以協助解決您的問題：</span><span class="sxs-lookup"><span data-stu-id="60405-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="60405-117">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="60405-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="60405-118">檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="60405-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="60405-119">檢閱[本文件](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的清單中的每個防止註冊和解決方法的常見錯誤。</span><span class="sxs-lookup"><span data-stu-id="60405-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="60405-120">[了解如何註冊 Microsoft Intune 中的 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="60405-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
    

