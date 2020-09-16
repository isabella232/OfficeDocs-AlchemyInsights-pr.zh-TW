---
title: 使用 Intune 在監督的 iOS 裝置上略過啟用鎖定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757291"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="a6906-102">使用 Intune 在監督的 iOS 裝置上略過啟用鎖定</span><span class="sxs-lookup"><span data-stu-id="a6906-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="a6906-103">在 iOS 裝置上略過啟用鎖定的功能，可讓您更輕鬆地從使用者啟用公司裝置上的啟用鎖定，然後離開公司。</span><span class="sxs-lookup"><span data-stu-id="a6906-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="a6906-104">跳過啟用鎖定的先決條件包括：</span><span class="sxs-lookup"><span data-stu-id="a6906-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="a6906-105">裝置是「受監督的」。</span><span class="sxs-lookup"><span data-stu-id="a6906-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="a6906-106">啟用鎖定已在 Intune 中使用 iOS 裝置限制原則成功啟用。</span><span class="sxs-lookup"><span data-stu-id="a6906-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="a6906-107">此外，如果略過啟用鎖定，您應：</span><span class="sxs-lookup"><span data-stu-id="a6906-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="a6906-108">實際擁有資料被擦除的裝置。</span><span class="sxs-lookup"><span data-stu-id="a6906-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="a6906-109">在您發布擦除命令之前，先複製程式碼。</span><span class="sxs-lookup"><span data-stu-id="a6906-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="a6906-110">**注意：** [擦除程式碼] 不區分大小寫，因此不需要 "-" 字元。</span><span class="sxs-lookup"><span data-stu-id="a6906-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="a6906-111">如需詳細資訊，請參閱 [以 Intune 在受監督的 iOS 裝置上略過啟用所訂](https://docs.microsoft.com/intune/device-activation-lock-bypass)。</span><span class="sxs-lookup"><span data-stu-id="a6906-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="a6906-112">**常見問題集**</span><span class="sxs-lookup"><span data-stu-id="a6906-112">**FAQ**</span></span>

<span data-ttu-id="a6906-113">問： **我已發布遠端動作來移除裝置上的公司資料，現在它停滯在擱置中的狀態。**</span><span class="sxs-lookup"><span data-stu-id="a6906-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="a6906-114">答：為了讓遠端動作順利完成，目標裝置必須連上網路且狀況良好。</span><span class="sxs-lookup"><span data-stu-id="a6906-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="a6906-115">在下列情況中，遠端動作會停留在擱置狀態達30天，或直到裝置在以下狀況中確認該命令為止：</span><span class="sxs-lookup"><span data-stu-id="a6906-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="a6906-116">沒有連線。</span><span class="sxs-lookup"><span data-stu-id="a6906-116">Does not have connectivity.</span></span>
- <span data-ttu-id="a6906-117">因 Intune 喪失其管理狀態。</span><span class="sxs-lookup"><span data-stu-id="a6906-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="a6906-118">如果您認為裝置已停止簽入，且無法移除公司資料，請選取 [刪除]。</span><span class="sxs-lookup"><span data-stu-id="a6906-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="a6906-119">[刪除] 會移除裝置記錄，所以它不會再出現在 Intune 裝置清單中。</span><span class="sxs-lookup"><span data-stu-id="a6906-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="a6906-120">若要讓裝置再次啟用，其使用者必須重新註冊裝置。</span><span class="sxs-lookup"><span data-stu-id="a6906-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="a6906-121">問： **為什麼我無法使用某些遠端動作？**</span><span class="sxs-lookup"><span data-stu-id="a6906-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="a6906-122">答：並非所有平臺都支援所有的遠端裝置動作。</span><span class="sxs-lookup"><span data-stu-id="a6906-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="a6906-123">下列遠端動作屬於平臺特定。</span><span class="sxs-lookup"><span data-stu-id="a6906-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="a6906-124">略過啟用鎖定（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="a6906-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="a6906-125">新開始（僅限 Windows）</span><span class="sxs-lookup"><span data-stu-id="a6906-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="a6906-126">遺失模式（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="a6906-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="a6906-127">定位裝置（僅限 iOS）</span><span class="sxs-lookup"><span data-stu-id="a6906-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="a6906-128">重新啟動 (僅限 Windows)</span><span class="sxs-lookup"><span data-stu-id="a6906-128">Restart (Windows only)</span></span>

<span data-ttu-id="a6906-129">如需每個動作的詳細資訊，請參閱 [可用的裝置動作](https://docs.microsoft.com/intune/device-management#available-device-actions)。</span><span class="sxs-lookup"><span data-stu-id="a6906-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>