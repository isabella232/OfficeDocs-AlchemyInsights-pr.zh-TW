---
title: 從裝置庫存移除 offboarded 或解除授權裝置時的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/11/2021
ms.locfileid: "52319170"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="d7f34-102">從裝置庫存移除 offboarded 或解除授權裝置時的問題</span><span class="sxs-lookup"><span data-stu-id="d7f34-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="d7f34-103">Microsoft Defender for Endpoint 目前不允許從裝置庫存手動移除 offboarded 或解除授權裝置的裝置記錄。</span><span class="sxs-lookup"><span data-stu-id="d7f34-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="d7f34-104">基於安全性的考慮，裝置會在入口網站中維持為歷史記錄，最多180天。</span><span class="sxs-lookup"><span data-stu-id="d7f34-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="d7f34-105">不過，裝置資料會根據您設定的保留期間來清除。</span><span class="sxs-lookup"><span data-stu-id="d7f34-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="d7f34-106">**附注：** Offboarded 或解除授權的裝置會在七天后自動切換到 **非** 使用中狀態。</span><span class="sxs-lookup"><span data-stu-id="d7f34-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="d7f34-107">此外，過去30天內非使用中的裝置不會考慮反映組織威脅的資料，也不會影響裝置的漏洞管理洩密分數或 Microsoft 安全分數。</span><span class="sxs-lookup"><span data-stu-id="d7f34-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="d7f34-108">如果您仍不想要在裝置庫存模式中查看特定裝置，請嘗試放置裝置標籤，以從裝置庫存模式中篩選出解除授權的裝置。</span><span class="sxs-lookup"><span data-stu-id="d7f34-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="d7f34-109">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="d7f34-109">For more information, see:</span></span>

[<span data-ttu-id="d7f34-110">Microsoft Defender for Endpoint service 中的下架裝置</span><span class="sxs-lookup"><span data-stu-id="d7f34-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="d7f34-111">威脅和弱點管理中的披露分數</span><span class="sxs-lookup"><span data-stu-id="d7f34-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="d7f34-112">修正 Microsoft Defender for Endpoint 中的狀況不良感應器</span><span class="sxs-lookup"><span data-stu-id="d7f34-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="d7f34-113">如何有效地使用標記 (第1部分) </span><span class="sxs-lookup"><span data-stu-id="d7f34-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="d7f34-114">如何有效地使用標記 (第2部分) </span><span class="sxs-lookup"><span data-stu-id="d7f34-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="d7f34-115">如何有效地使用標記 (第3部分) </span><span class="sxs-lookup"><span data-stu-id="d7f34-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




