---
title: 建立及管理裝置標籤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721677"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="22ce8-102">建立及管理裝置標籤</span><span class="sxs-lookup"><span data-stu-id="22ce8-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="22ce8-103">在裝置上新增標籤以建立邏輯群組關係。</span><span class="sxs-lookup"><span data-stu-id="22ce8-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="22ce8-104">裝置標籤支援網路的正確對應，使您能够附加不同的標籤以擷取内容，並作為事件的一部分啟用動態清單建立。</span><span class="sxs-lookup"><span data-stu-id="22ce8-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="22ce8-105">標籤可以用作裝置清單檢視中的篩檢，也可以用於對裝置進行分組。</span><span class="sxs-lookup"><span data-stu-id="22ce8-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="22ce8-106">有關裝置分組的詳細資訊，請參閱[建立和管理裝置標籤](/microsoft-365/security/defender-endpoint/machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="22ce8-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="22ce8-107">可以使用以下方法在裝置上新增標籤：</span><span class="sxs-lookup"><span data-stu-id="22ce8-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="22ce8-108">使用入口網站</span><span class="sxs-lookup"><span data-stu-id="22ce8-108">Using the portal</span></span>

- <span data-ttu-id="22ce8-109">設定登錄機碼值</span><span class="sxs-lookup"><span data-stu-id="22ce8-109">Setting a registry key value</span></span>
 
<span data-ttu-id="22ce8-110">**注意：** 從將標籤新增到裝置的時間，到其在裝置清單和裝置頁中的顯示可用的時間，會有一些延遲。</span><span class="sxs-lookup"><span data-stu-id="22ce8-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="22ce8-111">要使用 API 新增裝置標籤，請參閲[新增或移除裝置標籤 API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="22ce8-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="22ce8-112">使用入口網站新增和管理裝置標籤</span><span class="sxs-lookup"><span data-stu-id="22ce8-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="22ce8-113">選取要在其上管理標籤的裝置。</span><span class="sxs-lookup"><span data-stu-id="22ce8-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="22ce8-114">您可以從以下任何檢視中選取或搜尋裝置：</span><span class="sxs-lookup"><span data-stu-id="22ce8-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="22ce8-115">**安全性操作儀表板** - 從具有作用中警示的頂端裝置區段中選取裝置名稱。</span><span class="sxs-lookup"><span data-stu-id="22ce8-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="22ce8-116">**警示佇列** - 從警示佇列中選取裝置圖示旁邊的裝置名稱。</span><span class="sxs-lookup"><span data-stu-id="22ce8-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="22ce8-117">**裝置清單** - 從裝置清單中選取裝置名稱。</span><span class="sxs-lookup"><span data-stu-id="22ce8-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="22ce8-118">**搜尋方塊** - 從下拉式功能表中選取裝置並輸入裝置名稱。</span><span class="sxs-lookup"><span data-stu-id="22ce8-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="22ce8-119">您還可以透過檔案和 IP 檢視存取警示頁。</span><span class="sxs-lookup"><span data-stu-id="22ce8-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="22ce8-120">從回應動作列中選取 **管理標籤**。</span><span class="sxs-lookup"><span data-stu-id="22ce8-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="22ce8-121">輸入以尋找或建立標籤。</span><span class="sxs-lookup"><span data-stu-id="22ce8-121">Type to find or create tags.</span></span>

<span data-ttu-id="22ce8-122">新增至裝置檢視中的標籤，也會反映在裝置清單檢視中。</span><span class="sxs-lookup"><span data-stu-id="22ce8-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="22ce8-123">然後可以使用 [標籤] 篩選查看相關的裝置清單。</span><span class="sxs-lookup"><span data-stu-id="22ce8-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="22ce8-124">如需詳細資訊，請參閱，請參閱[建立和管理裝置標籤](/microsoft-365/security/defender-endpoint/machine-tags)。</span><span class="sxs-lookup"><span data-stu-id="22ce8-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>