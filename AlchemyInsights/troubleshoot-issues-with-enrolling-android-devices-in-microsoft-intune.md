---
title: 在 Microsoft Intune 中註冊 Android 裝置的問題疑難排解
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708989"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="fef29-102">在 Microsoft Intune 中註冊 Android 裝置的問題疑難排解</span><span class="sxs-lookup"><span data-stu-id="fef29-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="fef29-103">立即查看下列資源，以解決您的問題。</span><span class="sxs-lookup"><span data-stu-id="fef29-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="fef29-104">一些常見的問題和解決步驟：</span><span class="sxs-lookup"><span data-stu-id="fef29-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="fef29-105">**公司入口網站中的裝置未加密錯誤：** 較新版本的 Android （特別是從 v 7.0 開始）需要啟動密碼，以確保您的裝置已完全加密。</span><span class="sxs-lookup"><span data-stu-id="fef29-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="fef29-106">常見的解決方案是啟用啟動 pin 碼或完全加密裝置。</span><span class="sxs-lookup"><span data-stu-id="fef29-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="fef29-107">如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) 。</span><span class="sxs-lookup"><span data-stu-id="fef29-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="fef29-108">在 **intune 管理主控台中，裝置無法存回 intune 服務或顯示為「不良」：** 有些 Samsung 4.4 和5.5 裝置可能無法存回服務。</span><span class="sxs-lookup"><span data-stu-id="fef29-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="fef29-109">此問題有三種可能的解決方案：</span><span class="sxs-lookup"><span data-stu-id="fef29-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="fef29-110">手動開啟 Intune 公司入口網站應用程式，此應用程式會自動啟動裝置同步處理。</span><span class="sxs-lookup"><span data-stu-id="fef29-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="fef29-111">將裝置更新為 Android 6.0 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="fef29-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="fef29-112">停用 Samsung Smart Manager 管理 Intune 公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="fef29-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="fef29-113">如需這些問題和解決方法的詳細資訊，請參閱 [本檔](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) 。</span><span class="sxs-lookup"><span data-stu-id="fef29-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="fef29-114">**使用者授權類型無效** 或 **使用者名稱無法辨識錯誤：** 使用者必須被指派一個 Intune 或 EMS 授權。</span><span class="sxs-lookup"><span data-stu-id="fef29-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="fef29-115">檢查這些檔，以指派授權至： Office 系統管理中心或 Azure 入口網站。</span><span class="sxs-lookup"><span data-stu-id="fef29-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="fef29-116">其他可協助您解決問題的資源：</span><span class="sxs-lookup"><span data-stu-id="fef29-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="fef29-117">使用 [Intune 疑難排解入口網站](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) 來診斷及解決一般註冊失敗。</span><span class="sxs-lookup"><span data-stu-id="fef29-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="fef29-118">如需詳細資訊，請參閱 [本檔](https://docs.microsoft.com/intune/help-desk-operators) 。</span><span class="sxs-lookup"><span data-stu-id="fef29-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="fef29-119">請參閱 [本檔](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) ，以取得避免每個專案的註冊和解析度的常見錯誤清單。</span><span class="sxs-lookup"><span data-stu-id="fef29-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="fef29-120">[瞭解如何在 Microsoft Intune 中註冊 Android 裝置](https://docs.microsoft.com/intune/android-enroll)。</span><span class="sxs-lookup"><span data-stu-id="fef29-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
