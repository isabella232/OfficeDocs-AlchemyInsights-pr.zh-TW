---
title: 使用 Intune 查找遺失的 iOS 裝置
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434577"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="5130e-102">使用 Intune 查找遺失的 iOS 裝置</span><span class="sxs-lookup"><span data-stu-id="5130e-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="5130e-103">在 iOS 裝置上啟用遺失模式，可讓系統管理員在鎖屏上顯示訊息和連絡人電話號碼。</span><span class="sxs-lookup"><span data-stu-id="5130e-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="5130e-104">遺失模式啟用後，系統管理員可使用 [定位裝置] 動作來識別裝置的物理位置。</span><span class="sxs-lookup"><span data-stu-id="5130e-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="5130e-105">Intune 中的 [定位裝置] 動作可與 iOS 裝置搭配使用，以在地圖上顯示特定裝置的位置。</span><span class="sxs-lookup"><span data-stu-id="5130e-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="5130e-106">若要使用此動作，您的 iOS 裝置必須處於：</span><span class="sxs-lookup"><span data-stu-id="5130e-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="5130e-107">監督模式</span><span class="sxs-lookup"><span data-stu-id="5130e-107">Supervised mode</span></span>
- <span data-ttu-id="5130e-108">遺失模式</span><span class="sxs-lookup"><span data-stu-id="5130e-108">Lost mode</span></span>

<span data-ttu-id="5130e-109">如需詳細資訊，請參閱[使用 Intune在 iOS/iPadOS 裝置上啟用遺失模式](https://docs.microsoft.com/intune/device-lost-mode) 以及 [使用 Intune 尋找遺失或失竊的 iOS/iPadOS 裝置](https://docs.microsoft.com/intune/device-locate)。</span><span class="sxs-lookup"><span data-stu-id="5130e-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="5130e-110">**常見問題集**</span><span class="sxs-lookup"><span data-stu-id="5130e-110">**FAQ**</span></span>

<span data-ttu-id="5130e-111">問：我已發布遠端動作來移除裝置上的公司資料，現在它停滯在擱置中的狀態。</span><span class="sxs-lookup"><span data-stu-id="5130e-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="5130e-112">答：為了讓遠端動作順利完成，目標裝置必須連上網路且狀況良好。</span><span class="sxs-lookup"><span data-stu-id="5130e-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="5130e-113">在下列情況中，遠端動作會停留在擱置狀態達30天，或直到裝置確認該命令為止：</span><span class="sxs-lookup"><span data-stu-id="5130e-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="5130e-114">當裝置離線。</span><span class="sxs-lookup"><span data-stu-id="5130e-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="5130e-115">當裝置因 Intune 喪失其管理狀態。</span><span class="sxs-lookup"><span data-stu-id="5130e-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="5130e-116">如果您認為裝置已停止簽入，且無法移除公司資料，請選取 [刪除]。</span><span class="sxs-lookup"><span data-stu-id="5130e-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="5130e-117">[刪除] 會移除裝置記錄，所以它不會再出現在 Intune 裝置清單中。</span><span class="sxs-lookup"><span data-stu-id="5130e-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="5130e-118">如果裝置再次啟動，使用者將必須重新註冊。</span><span class="sxs-lookup"><span data-stu-id="5130e-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="5130e-119">問：為什麼我無法使用某些遠端動作？</span><span class="sxs-lookup"><span data-stu-id="5130e-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="5130e-120">答：並非所有平臺都支援所有的遠端裝置動作。</span><span class="sxs-lookup"><span data-stu-id="5130e-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="5130e-121">下列遠端動作屬於平台特定，因此僅適用于指定的平台。</span><span class="sxs-lookup"><span data-stu-id="5130e-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="5130e-122">略過啟用鎖定（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="5130e-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="5130e-123">新開始（僅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="5130e-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="5130e-124">遺失模式（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="5130e-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="5130e-125">定位裝置（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="5130e-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="5130e-126">重新啟動 (僅限 Windows)</span><span class="sxs-lookup"><span data-stu-id="5130e-126">Restart (Windows only)</span></span>

<span data-ttu-id="5130e-127">如需每個動作的詳細資訊，請參閱 [可用的裝置動作](https://docs.microsoft.com/intune/device-management#available-device-actions)。</span><span class="sxs-lookup"><span data-stu-id="5130e-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>