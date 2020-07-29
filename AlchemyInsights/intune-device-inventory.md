---
title: Intune 裝置庫存
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
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434581"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="3f245-102">Intune 裝置庫存</span><span class="sxs-lookup"><span data-stu-id="3f245-102">Intune Device Inventory</span></span>

<span data-ttu-id="3f245-103">設備刀鋒在 Intune 管理中，為每個設備提供管理員深入解析。</span><span class="sxs-lookup"><span data-stu-id="3f245-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="3f245-104">顯示的資訊包括：硬體、發現的應用程式、裝置合規性狀態和裝置設定狀態。</span><span class="sxs-lookup"><span data-stu-id="3f245-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="3f245-105">硬體和發現的應用程式的庫存資料以每七天為週期收集。</span><span class="sxs-lookup"><span data-stu-id="3f245-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="3f245-106">所報告的硬體的應用程式和特定元素因設備作業系統以及設備是個人所有還是公司所有而有所不同。</span><span class="sxs-lookup"><span data-stu-id="3f245-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="3f245-107">如需詳細資訊，請參閱[在 Intune 中查看裝置詳細資料](https://docs.microsoft.com/intune/device-inventory)。</span><span class="sxs-lookup"><span data-stu-id="3f245-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="3f245-108">**常見問題集**</span><span class="sxs-lookup"><span data-stu-id="3f245-108">**FAQ**</span></span>

<span data-ttu-id="3f245-109">問：我沒有收到 Intune 註冊的 Windows 裝置上的應用程式完整庫存清單。</span><span class="sxs-lookup"><span data-stu-id="3f245-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="3f245-110">為什麼？</span><span class="sxs-lookup"><span data-stu-id="3f245-110">Why not?</span></span>

<span data-ttu-id="3f245-111">答：目前新式應用程式只被列在識別為企業裝置的 Windows 10 PC 上。</span><span class="sxs-lookup"><span data-stu-id="3f245-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="3f245-112">Intune 不收集安裝在這些裝置上的 Win32 應用程式相關資訊。</span><span class="sxs-lookup"><span data-stu-id="3f245-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="3f245-113">Q：為什麼不從所有裝置收集電話號碼？</span><span class="sxs-lookup"><span data-stu-id="3f245-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="3f245-114">A：例如，當執行行動裝置庫存報告時，Intune 中被歸類為企業設備的電話不會被識別為完整的電話號碼。</span><span class="sxs-lookup"><span data-stu-id="3f245-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="3f245-115">自帶裝置電話號碼總是用星號（\*\*\*\*）部分遮罩，並且只顯示最後四位數。</span><span class="sxs-lookup"><span data-stu-id="3f245-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>