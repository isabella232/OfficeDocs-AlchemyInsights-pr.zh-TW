---
title: 在 Microsoft Intune 中對 Windows 裝置的註冊問題進行疑難排解
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
ms.openlocfilehash: fa48b76fb49cdeef0734e77520c9bf95c150f317
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353528"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="0ac79-102">在 Microsoft Intune 中對 Windows 裝置的註冊問題進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="0ac79-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="0ac79-103">請查看下面所列的資源, 立即解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="0ac79-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="0ac79-104">一些常見的錯誤訊息和解決步驟:</span><span class="sxs-lookup"><span data-stu-id="0ac79-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="0ac79-105">**無法安裝軟體, 0x80cf4017:** 您的帳戶憑證已過期。</span><span class="sxs-lookup"><span data-stu-id="0ac79-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="0ac79-106">在 Intune 管理主控台中重新下載電腦用戶端軟體套件。</span><span class="sxs-lookup"><span data-stu-id="0ac79-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="0ac79-107">如需詳細資訊, 請參閱本檔。</span><span class="sxs-lookup"><span data-stu-id="0ac79-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="0ac79-108">**錯誤碼 0x801c0003:** 在下列案例中, 可能會發生此錯誤:</span><span class="sxs-lookup"><span data-stu-id="0ac79-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
1. <span data-ttu-id="0ac79-109">使用者所註冊的裝置數目超過裝置限制。</span><span class="sxs-lookup"><span data-stu-id="0ac79-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="0ac79-110">請查看這些檔, 以[移除裝置](https://docs.microsoft.com/intune/devices-wipe)或[變更裝置限制](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)。</span><span class="sxs-lookup"><span data-stu-id="0ac79-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

2. <span data-ttu-id="0ac79-111">[使用者可以將裝置加入 Azure AD] 設定為 "none"。</span><span class="sxs-lookup"><span data-stu-id="0ac79-111">"Users may join devices to Azure AD" is set to "none".</span></span> <span data-ttu-id="0ac79-112">將它設為 [所有] 或 [選取使用者]。</span><span class="sxs-lookup"><span data-stu-id="0ac79-112">Set it to all or select users.</span></span> <span data-ttu-id="0ac79-113">如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings)。</span><span class="sxs-lookup"><span data-stu-id="0ac79-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

3. <span data-ttu-id="0ac79-114">裝置已由另一位使用者註冊。</span><span class="sxs-lookup"><span data-stu-id="0ac79-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="0ac79-115">如果是這種情況, 請從 Azure Intune 主控台移除裝置, 或先手動取消註冊裝置, 再重試。</span><span class="sxs-lookup"><span data-stu-id="0ac79-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

4. <span data-ttu-id="0ac79-116">裝置是 Windows 10 家用版。</span><span class="sxs-lookup"><span data-stu-id="0ac79-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="0ac79-117">只有 Windows 10 專業版、教育版和企業版 Sku 可以加入 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="0ac79-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="0ac79-118">可協助您解決問題的其他資源:</span><span class="sxs-lookup"><span data-stu-id="0ac79-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="0ac79-119">使用[Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade)來診斷和解決常見的註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="0ac79-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="0ac79-120">如需詳細資訊, 請參閱[本檔](https://docs.microsoft.com/intune/help-desk-operators)。</span><span class="sxs-lookup"><span data-stu-id="0ac79-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="0ac79-121">請查看這些檔, 以取得防止每個專案的註冊和解析度的常見錯誤清單:[疑難排解指南](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune)和[疑難排解 doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="0ac79-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="0ac79-122">[瞭解如何在 Microsoft Intune 中註冊 Windows 裝置](https://docs.microsoft.com/intune/windows-enroll)。</span><span class="sxs-lookup"><span data-stu-id="0ac79-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
