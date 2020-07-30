---
title: 從 Intune 重設裝置 pin/密碼
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431475"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="34d40-102">從 Intune 重設裝置 pin/密碼</span><span class="sxs-lookup"><span data-stu-id="34d40-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="34d40-103">您可以使用 [移除密碼] 動作，移除密碼或強制使用者在 Intune 中為執行 iOS 或 Android 的裝置建立新的密碼。</span><span class="sxs-lookup"><span data-stu-id="34d40-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="34d40-104">只有特定的作業系統類型和工作設定檔類型支援此動作。</span><span class="sxs-lookup"><span data-stu-id="34d40-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="34d40-105">如需支援的平台以及如何觸發重設密碼動作的詳細資訊，請參閱[在 Intune 中重設或移除裝置密碼](https://docs.microsoft.com/intune/device-passcode-reset)。</span><span class="sxs-lookup"><span data-stu-id="34d40-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="34d40-106">在執行 Windows 10 行動裝置版作業系統的裝置上，您可以使用 Pin 重設動作，將現有的 pin 重設為新的值。</span><span class="sxs-lookup"><span data-stu-id="34d40-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="34d40-107">這允許使用者解除鎖定裝置，並視需要設定新的 pin。</span><span class="sxs-lookup"><span data-stu-id="34d40-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="34d40-108">如需詳細資訊，請參閱[使用 Intune 重設 Windows 裝置上的密碼](https://docs.microsoft.com/intune/device-windows-pin-reset)。</span><span class="sxs-lookup"><span data-stu-id="34d40-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>