---
title: 疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8c5e7cc502d016ad658383685523dc240dfb4dc6
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661507"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="2bf5e-102">疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置</span><span class="sxs-lookup"><span data-stu-id="2bf5e-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="2bf5e-103">請檢閱下面列出現在解決問題的資源。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="2bf5e-104">一些常見的錯誤訊息和解決步驟：</span><span class="sxs-lookup"><span data-stu-id="2bf5e-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="2bf5e-p101">**無法安裝軟體、 0x80cf4017:** 帳戶憑證已過期。重新下載 Intune 系統管理主控台的電腦用戶端軟體封裝。請檢閱此文件的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="2bf5e-108">**錯誤碼 0x801c0003:** 在下列情況會發生錯誤：</span><span class="sxs-lookup"><span data-stu-id="2bf5e-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="2bf5e-p102">使用者有多個裝置註冊於裝置限制。檢閱這些文件[中移除裝置](https://docs.microsoft.com/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="2bf5e-p103">「 使用者可能會加入裝置 Azure AD"設為"none"。將它設為所有或選取使用者。請檢閱[此文件](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="2bf5e-p104">裝置已經由另一個使用者註冊。如果這是大小寫、 Azure Intune 主控台中移除裝置或手動重新嘗試之前 unenroll 裝置。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="2bf5e-p105">裝置首頁 Windows 10。僅限 Windows 10 專業人員、 教育版與企業 Sku 可加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="2bf5e-118">若要協助解決問題的其他資源：</span><span class="sxs-lookup"><span data-stu-id="2bf5e-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="2bf5e-p106">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷及解決常見的註冊失敗。請檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="2bf5e-121">檢閱這些文件的每個防止註冊和解決方法的常見錯誤的清單：[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)及[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="2bf5e-122">[解如何註冊 Microsoft Intune 中的 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="2bf5e-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
  

