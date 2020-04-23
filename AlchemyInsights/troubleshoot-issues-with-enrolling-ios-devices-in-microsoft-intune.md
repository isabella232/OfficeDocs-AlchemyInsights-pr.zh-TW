---
title: 在 Microsoft Intune 中登記 iOS 裝置的問題疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736149"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="4b473-102">在 Microsoft Intune 中登記 iOS 裝置的問題疑難排解</span><span class="sxs-lookup"><span data-stu-id="4b473-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="4b473-103">立即查看下列資源，以解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="4b473-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="4b473-104">一些常見的錯誤訊息和解決步驟：</span><span class="sxs-lookup"><span data-stu-id="4b473-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="4b473-105">已**達到裝置 Cap**使用者已註冊的裝置數目超過裝置限制。</span><span class="sxs-lookup"><span data-stu-id="4b473-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="4b473-106">請檢查這些檔，以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="4b473-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="4b473-107">**不支援此服務。無註冊原則：** 必須設定或更新 Apple Push Notification 服務（apn）。</span><span class="sxs-lookup"><span data-stu-id="4b473-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="4b473-108">如需如何執行此作業的指示，請參閱[本檔](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)。</span><span class="sxs-lookup"><span data-stu-id="4b473-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="4b473-109">**使用者授權類型無效或無法識別使用者名稱：** 使用者必須被指派 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="4b473-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="4b473-110">檢查這些檔，以指派授權至： [Office 系統管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="4b473-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="4b473-111">其他可協助您解決問題的資源：</span><span class="sxs-lookup"><span data-stu-id="4b473-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="4b473-112">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決一般註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="4b473-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="4b473-113">如需詳細資訊，請參閱[本檔](https://docs.microsoft.com/intune/help-desk-operators)。</span><span class="sxs-lookup"><span data-stu-id="4b473-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="4b473-114">請查看這些檔，以取得阻止每個專案之註冊和解析度的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="4b473-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="4b473-115">[瞭解如何在 Microsoft Intune 中註冊 iOS 裝置](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="4b473-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

