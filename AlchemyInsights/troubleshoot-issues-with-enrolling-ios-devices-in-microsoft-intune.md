---
title: 疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: bdbfe7bae00a4c5cfa0edbe9a37522cc98e52401
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36506910"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="0bc78-102">疑難排解問題註冊 Microsoft Intune 中的 iOS 裝置</span><span class="sxs-lookup"><span data-stu-id="0bc78-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="0bc78-103">請先檢閱下列資源以立即解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="0bc78-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="0bc78-104">一些常見的錯誤訊息及解決步驟：</span><span class="sxs-lookup"><span data-stu-id="0bc78-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="0bc78-105">**達到裝置限制**使用者有多個裝置註冊比裝置的限制。</span><span class="sxs-lookup"><span data-stu-id="0bc78-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0bc78-106">檢閱這些文件以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)，或[變更裝置的限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="0bc78-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="0bc78-107">不支援**此服務。沒有註冊的原則：** Apple 推播通知服務 (APNS) 需要設定或更新。</span><span class="sxs-lookup"><span data-stu-id="0bc78-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="0bc78-108">檢閱[本文件](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get)如需如何執行這項作業的指示。</span><span class="sxs-lookup"><span data-stu-id="0bc78-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="0bc78-109">**使用者授權類型不正確或無法辨識的使用者名稱：** 使用者需要已獲得 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="0bc78-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="0bc78-110">檢閱這些文件以透過將授權指派： [Office 系統管理中心](https://docs.microsoft.com/intune/licenses-assign)或[Azure 入口網站](https://docs.microsoft.com/azure/active-directory/license-users-groups)。</span><span class="sxs-lookup"><span data-stu-id="0bc78-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="0bc78-111">其他資源，可以協助解決您的問題：</span><span class="sxs-lookup"><span data-stu-id="0bc78-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0bc78-112">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="0bc78-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0bc78-113">檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="0bc78-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="0bc78-114">檢閱這些文件的每個防止註冊和解決方法的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="0bc78-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="0bc78-115">[了解如何註冊 Microsoft Intune 中的 iOS 裝置](https://docs.microsoft.com/intune/ios-enroll)。</span><span class="sxs-lookup"><span data-stu-id="0bc78-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

