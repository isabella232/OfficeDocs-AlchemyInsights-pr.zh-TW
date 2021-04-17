---
title: 疑難排解現有監視器
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824570"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="fe4e5-102">疑難排解現有監視器</span><span class="sxs-lookup"><span data-stu-id="fe4e5-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="fe4e5-103">請嘗試這些解決方案來疑難排解監視器。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="fe4e5-104">**重新整理監視器的顯示：**</span><span class="sxs-lookup"><span data-stu-id="fe4e5-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="fe4e5-105">同步選取下列機碼： Windows 鍵 + Ctrl + Shift + B。這將會重新整理與您的圖形驅動程式的通訊。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="fe4e5-106">您的監視器會稍閃閃爍，並在幾秒鐘後傳回回來。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="fe4e5-107">**監視硬體疑難排解：**</span><span class="sxs-lookup"><span data-stu-id="fe4e5-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="fe4e5-108">拔除連接電腦與監視器的纜線，然後插回。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="fe4e5-109">中斷任何非必要裝置與電腦 (例如介面卡或 Dock) 的連接。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="fe4e5-110">**如果您最近在您的電腦上安裝更新，您可以復原您的顯示驅動程式：**</span><span class="sxs-lookup"><span data-stu-id="fe4e5-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="fe4e5-111">選取 [ **開始**]，輸入 [ **裝置管理員**]，然後從 [結果] 中選取 [ **裝置管理員** ]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="fe4e5-112">展開 [ **顯示配接器** ] 區段中，以滑鼠右鍵按一下您的顯示配接器，and 選取 [ **屬性**]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="fe4e5-113">流覽至 [ **驅動程式** ] 索引標籤，然後選取 [ **還原驅動程式**]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="fe4e5-114">附注：如果這不是可用或變暗，請從下列選項中選取 [ **否** ]，以移至下一個步驟。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="fe4e5-115">您可能需要先重新開機電腦，這些變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="fe4e5-116">**卸載並重新安裝您的顯示驅動程式：**</span><span class="sxs-lookup"><span data-stu-id="fe4e5-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="fe4e5-117">選取 [ **開始**]，輸入 [ **裝置管理員**]，然後從 [結果] 中選取 [ **裝置管理員** ]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="fe4e5-118">展開 [ **顯示配接器** ] 區段中，以滑鼠右鍵按一下您的顯示配接器，and 選取 [ **卸載裝置**]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="fe4e5-119">選取 [ **刪除此裝置的驅動程式軟體** ] 旁邊的方塊，然後選取 [ **卸載**]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="fe4e5-120">附注：您可能會在此階段要求您重新開機電腦。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="fe4e5-121">重新開機之前，請務必記下來餘下的指示。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="fe4e5-122">再次開啟 [裝置管理員]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="fe4e5-123">展開 [ **顯示配接器** ] 區段，以滑鼠右鍵按一下您的顯示配接器，然後選取 [ **更新驅動程式**]。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="fe4e5-124">選取 [ **自動搜尋更新驅動程式軟體** ]，並遵循安裝指示。</span><span class="sxs-lookup"><span data-stu-id="fe4e5-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>