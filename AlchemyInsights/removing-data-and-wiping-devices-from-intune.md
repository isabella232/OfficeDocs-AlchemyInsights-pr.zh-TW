---
title: 從 Intune 中移除數據和抹除裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701274"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="fc397-102">從 Intune 中移除數據和抹除裝置</span><span class="sxs-lookup"><span data-stu-id="fc397-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="fc397-103">設備淘汰和設備抹除遠端操作可用於移除 Intune 管理的公司資料，或執行出廠預設並將設備恢復為其默認設置。</span><span class="sxs-lookup"><span data-stu-id="fc397-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="fc397-104">登入 Microsoft 365 裝置管理，然後移至 **裝置** > **所有裝置**。</span><span class="sxs-lookup"><span data-stu-id="fc397-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="fc397-105">選取您要抹除的裝置。</span><span class="sxs-lookup"><span data-stu-id="fc397-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="fc397-106">選取您要執行的遠端抹除類型。</span><span class="sxs-lookup"><span data-stu-id="fc397-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="fc397-107">[淘汰] 只會刪除組織資訊，而完整的抹除則會將裝置還原為出廠預設。</span><span class="sxs-lookup"><span data-stu-id="fc397-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="fc397-108">選取 **[是]** 加以確認。</span><span class="sxs-lookup"><span data-stu-id="fc397-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="fc397-109">裝置動作狀態將顯示為 [停用擱置]，直到抹除完成為止。</span><span class="sxs-lookup"><span data-stu-id="fc397-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="fc397-110">操作完成之後，您將不會再在受管理裝置清單中看到該行動裝置。</span><span class="sxs-lookup"><span data-stu-id="fc397-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="fc397-111">**附註** 無法從加入 Azure AD 的裝置中移除公司資料。</span><span class="sxs-lookup"><span data-stu-id="fc397-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="fc397-112">如需淘汰和抹除動作影響的完整詳細資料 (包括保留內容和刪除內容)，請參閱 [使用 [擦除]、[淘汰] 或手動撤銷裝置的註冊來移除裝置](https://docs.microsoft.com/intune/devices-wipe)。</span><span class="sxs-lookup"><span data-stu-id="fc397-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="fc397-113">若要清除 macOS 裝置上的所有資料，請參閱 [清除 macOS 裝置中的所有資料](https://docs.microsoft.com/intune/device-erase)。</span><span class="sxs-lookup"><span data-stu-id="fc397-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>