---
title: Defender 端點檢查感應器狀態
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/24/2021
ms.locfileid: "52627233"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="5c71f-102">Defender 端點檢查感應器狀態</span><span class="sxs-lookup"><span data-stu-id="5c71f-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="5c71f-103">**有感應器問題的裝置** 磚位於安全性作業儀表板上。</span><span class="sxs-lookup"><span data-stu-id="5c71f-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="5c71f-104">此磚提供有關個別裝置提供感應器資料和與適用於端點的 Defender 服務通訊的能力之資訊。</span><span class="sxs-lookup"><span data-stu-id="5c71f-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="5c71f-105">它報告需要注意的裝置數量，並協助您識別有問題的裝置並採取措施修正已知問題。</span><span class="sxs-lookup"><span data-stu-id="5c71f-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="5c71f-106">磚上的兩個狀態指示器提供有關未正確向服務報告的裝置數量之資訊：</span><span class="sxs-lookup"><span data-stu-id="5c71f-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="5c71f-107">**設定錯誤** 可能部分向適用於端點的 Defender 服務報告感應器資料並且可能存在需要修正的設定錯誤之裝置。</span><span class="sxs-lookup"><span data-stu-id="5c71f-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="5c71f-108">**閒置中** 過去一個月內超過 7 天未向適用於端點的 Defender 服務報告的裝置。</span><span class="sxs-lookup"><span data-stu-id="5c71f-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="5c71f-109">按一下任何群組都會將您導向至裝置清單，並根據您的選擇進行篩選。</span><span class="sxs-lookup"><span data-stu-id="5c71f-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="5c71f-110">在裝置清單中，可以按以下狀態篩選健康情況狀態清單：</span><span class="sxs-lookup"><span data-stu-id="5c71f-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="5c71f-111">**作用中** 不斷向適用於端點的 Defender 服務報告的裝置。</span><span class="sxs-lookup"><span data-stu-id="5c71f-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="5c71f-112">**設定錯誤** 可能部分向適用於端點的 Defender 服務報告感應器資料但存在需要修正的設定錯誤之裝置。</span><span class="sxs-lookup"><span data-stu-id="5c71f-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="5c71f-113">設定錯誤的裝置可能存在以下一個或多個問題：</span><span class="sxs-lookup"><span data-stu-id="5c71f-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="5c71f-114">無感應器資料 - 裝置已停止傳送感應器資料。</span><span class="sxs-lookup"><span data-stu-id="5c71f-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="5c71f-115">裝置可以觸發有限的警示。</span><span class="sxs-lookup"><span data-stu-id="5c71f-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="5c71f-116">通訊受損 - 與裝置通訊的能力受損。</span><span class="sxs-lookup"><span data-stu-id="5c71f-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="5c71f-117">傳送檔案進行深入分析、封鎖檔案、將裝置與網路隔離以及其他需要與裝置通訊的動作可能無法運行。</span><span class="sxs-lookup"><span data-stu-id="5c71f-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="5c71f-118">**閒置中** 已停止向適用於端點的 Defender 服務報告的裝置。</span><span class="sxs-lookup"><span data-stu-id="5c71f-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="5c71f-119">您可以使用匯出功能以 CSV 格式下載整個清單。</span><span class="sxs-lookup"><span data-stu-id="5c71f-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="5c71f-120">如需詳細資訊，請參閱[檢查適用於端點的 Microsoft Defender 中的感應器健全狀態](/microsoft-365/security/defender-endpoint/check-sensor-status)。</span><span class="sxs-lookup"><span data-stu-id="5c71f-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="5c71f-121">如需導致裝置處於裝置狀態或設定錯誤的原因之詳細資訊，請參閱 [修正適用於端點的 Microsoft Defender 中的不良感應器](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)。</span><span class="sxs-lookup"><span data-stu-id="5c71f-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
