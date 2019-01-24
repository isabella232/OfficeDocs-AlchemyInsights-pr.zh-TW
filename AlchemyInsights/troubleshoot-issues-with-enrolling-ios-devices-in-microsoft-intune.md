---
title: 疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460959"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="f4275-102">疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置</span><span class="sxs-lookup"><span data-stu-id="f4275-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="f4275-103">請檢閱下面列出現在解決問題的資源。</span><span class="sxs-lookup"><span data-stu-id="f4275-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f4275-104">一些常見的錯誤訊息和解決步驟：</span><span class="sxs-lookup"><span data-stu-id="f4275-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="f4275-p101">**連線至裝置限制**使用者有多個裝置註冊於裝置限制。檢閱這些文件[中移除裝置](https://docs.microsoft.com/en-us/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="f4275-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="f4275-p102">不支援**此新服務。註冊無原則：** Apple 推入通知服務 (APNS) 需要設定或更新。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get)如需如何執行作業的指示。</span><span class="sxs-lookup"><span data-stu-id="f4275-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="f4275-p103">**使用者授權類型不正確或無法辨識的使用者名稱：** 使用者必須被指派 Intune 或 EMS 授權。檢閱這些文件以透過將授權指派： [Office 系統管理中心](https://docs.microsoft.com/en-us/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="f4275-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="f4275-111">若要協助解決問題的其他資源：</span><span class="sxs-lookup"><span data-stu-id="f4275-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f4275-p104">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/en-us/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="f4275-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f4275-114">檢閱這些文件的每個防止註冊和解決方法的常見錯誤的清單：[疑難排解指南](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune)及[疑難排解 doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="f4275-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="f4275-115">[解如何註冊 Microsoft Intune 中的 iOS 裝置](https://docs.microsoft.com/en-us/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="f4275-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

