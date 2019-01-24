---
title: 疑難排解問題註冊 Microsoft Intune 在 Android 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 2f4fc434128ebe7323f0b8c08aec3be82112bbda
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460534"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="005db-102">疑難排解問題註冊 Microsoft Intune 在 Android 裝置</span><span class="sxs-lookup"><span data-stu-id="005db-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="005db-103">請檢閱下面列出現在解決問題的資源。</span><span class="sxs-lookup"><span data-stu-id="005db-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="005db-104">部分一般問題與解決步驟：</span><span class="sxs-lookup"><span data-stu-id="005db-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="005db-p101">**裝置未加密的公司入口網站中的錯誤：** Android，特別開頭 v7.0、 較新版本需要啟動密碼以確定您的裝置已完全加密。若要啟用啟動 pin 或完全加密裝置是常見的方案。請檢閱[本文件](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="005db-p101">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted. Common solutions are to enable a startup pin or fully encrypt the device. Review [this document](https://docs.microsoft.com/en-us/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span> 
  
 <span data-ttu-id="005db-p102">**裝置無法檢查使用 Intune 服務或 Intune 系統管理主控台中顯示為"Unhealthy":** 某些 Samsung 4.4 和 5.5 裝置可能會檢查服務。有這個問題 3 可能的解決方案：</span><span class="sxs-lookup"><span data-stu-id="005db-p102">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service. There are 3 possible solutions to this issue:</span></span> 
  
1. <span data-ttu-id="005db-110">以手動方式開啟 Intune 的公司入口網站應用程式，將會自動啟動裝置同步處理。</span><span class="sxs-lookup"><span data-stu-id="005db-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>
    
2. <span data-ttu-id="005db-111">更新裝置 Android 6.0 或更高。</span><span class="sxs-lookup"><span data-stu-id="005db-111">Update the device to Android 6.0 or higher.</span></span>
    
3. <span data-ttu-id="005db-p103">停用 Samsung 智慧管理員從管理 Intune 的公司入口網站。請檢閱[本文件](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console)如需這些問題及解決方法的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="005db-p103">Disable Samsung Smart Manager from managing the Intune Company Portal. Review [this document](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span> 
    
 <span data-ttu-id="005db-p104">**使用者授權類型不正確**或**使用者名稱不會辨識錯誤：** 使用者必須被指派 Intune 或 EMS 授權。檢閱這些文件以透過將授權指派： Office 系統管理中心或 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="005db-p104">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span> 
  
<span data-ttu-id="005db-116">若要協助解決問題的其他資源：</span><span class="sxs-lookup"><span data-stu-id="005db-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="005db-p105">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="005db-p105">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="005db-119">請檢閱[本文件](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune)的每個防止註冊和解決方法的常見錯誤的清單。</span><span class="sxs-lookup"><span data-stu-id="005db-119">Review [this document](https://docs.microsoft.com/en-us/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span> 
    
3. <span data-ttu-id="005db-120">[解如何註冊 Microsoft Intune 在 Android 裝置](https://docs.microsoft.com/en-us/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="005db-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/android-enroll).</span></span>
    

