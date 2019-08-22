---
title: 疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: be66135b80f32f78266ef2b6a7b3f5b30e24d5fc
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559652"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="588c1-102">疑難排解問題註冊 Microsoft Intune 中的 Windows 裝置</span><span class="sxs-lookup"><span data-stu-id="588c1-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="588c1-103">請先檢閱下列資源以立即解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="588c1-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="588c1-104">一些常見的錯誤訊息及解決步驟：</span><span class="sxs-lookup"><span data-stu-id="588c1-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="588c1-105">**無法安裝軟體，0x80cf4017:** 您的帳戶憑證已過期。</span><span class="sxs-lookup"><span data-stu-id="588c1-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="588c1-106">重新下載 Intune 管理主控台的電腦用戶端軟體封裝。</span><span class="sxs-lookup"><span data-stu-id="588c1-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="588c1-107">檢閱此文件的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="588c1-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="588c1-108">**錯誤碼 0x801c0003:** 在下列案例中，會發生錯誤：</span><span class="sxs-lookup"><span data-stu-id="588c1-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="588c1-109">使用者有多個裝置註冊比裝置的限制。</span><span class="sxs-lookup"><span data-stu-id="588c1-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="588c1-110">檢閱這些文件以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)，或[變更裝置的限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="588c1-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="588c1-111">「 使用者可能會加入裝置到 Azure AD 」 設為"none"。</span><span class="sxs-lookup"><span data-stu-id="588c1-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="588c1-112">將它設為所有或選取使用者。</span><span class="sxs-lookup"><span data-stu-id="588c1-112">Set it to all or select users.</span></span> <span data-ttu-id="588c1-113">檢閱[此文件](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="588c1-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="588c1-114">由其他使用者已經註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="588c1-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="588c1-115">如果是這種情況，若要從 Azure Intune 主控台移除裝置，或手動重新嘗試之前取消裝置。</span><span class="sxs-lookup"><span data-stu-id="588c1-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="588c1-116">裝置是 Windows 10 家用版。</span><span class="sxs-lookup"><span data-stu-id="588c1-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="588c1-117">僅限 Windows 10 專業版、 教育版和企業 Sku 可加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="588c1-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="588c1-118">其他資源，可以協助解決您的問題：</span><span class="sxs-lookup"><span data-stu-id="588c1-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="588c1-119">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="588c1-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="588c1-120">檢閱[本文件](https://docs.microsoft.com/intune/help-desk-operators)如需詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="588c1-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="588c1-121">檢閱這些文件的每個防止註冊和解決方法的常見錯誤清單：[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="588c1-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="588c1-122">[了解如何註冊 Microsoft Intune 中的 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="588c1-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
