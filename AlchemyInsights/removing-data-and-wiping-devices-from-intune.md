---
title: 從 Intune 中移除數據和抹除裝置
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434580"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="c5349-102">從 Intune 中移除數據和抹除裝置</span><span class="sxs-lookup"><span data-stu-id="c5349-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="c5349-103">設備淘汰和設備抹除遠端操作可用於移除 Intune 管理的公司資料，或執行出廠預設並將設備恢復為其默認設置。</span><span class="sxs-lookup"><span data-stu-id="c5349-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="c5349-104">登入 Microsoft 365 裝置管理，然後移至 **裝置** > **所有裝置**。</span><span class="sxs-lookup"><span data-stu-id="c5349-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="c5349-105">選取您要抹除的裝置。</span><span class="sxs-lookup"><span data-stu-id="c5349-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="c5349-106">選取您要執行的遠端抹除類型。</span><span class="sxs-lookup"><span data-stu-id="c5349-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="c5349-107">[淘汰] 只會刪除組織資訊，而完整的抹除則會將裝置還原為出廠預設。</span><span class="sxs-lookup"><span data-stu-id="c5349-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="c5349-108">選取 **[是]** 加以確認。</span><span class="sxs-lookup"><span data-stu-id="c5349-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="c5349-109">裝置動作狀態將顯示為 [停用擱置]，直到抹除完成為止。</span><span class="sxs-lookup"><span data-stu-id="c5349-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="c5349-110">操作完成之後，您將不會再在受管理裝置清單中看到該行動裝置。</span><span class="sxs-lookup"><span data-stu-id="c5349-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="c5349-111">**附註** 無法從加入 Azure AD 的裝置中移除公司資料。</span><span class="sxs-lookup"><span data-stu-id="c5349-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="c5349-112">如需淘汰和抹除動作影響的完整詳細資料 (包括保留內容和刪除內容)，請參閱 [使用 [擦除]、[淘汰] 或手動撤銷裝置的註冊來移除裝置](https://docs.microsoft.com/intune/devices-wipe)。</span><span class="sxs-lookup"><span data-stu-id="c5349-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="c5349-113">若要清除 macOS 裝置上的所有資料，請參閱 [清除 macOS 裝置中的所有資料](https://docs.microsoft.com/intune/device-erase)。</span><span class="sxs-lookup"><span data-stu-id="c5349-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>