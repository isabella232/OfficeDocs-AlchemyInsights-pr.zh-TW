---
title: 疑難排解現有監視器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738560"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="78306-102">疑難排解現有的監視器</span><span class="sxs-lookup"><span data-stu-id="78306-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="78306-103">請嘗試這些解決方案來疑難排解監視器。</span><span class="sxs-lookup"><span data-stu-id="78306-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="78306-104">**重新整理您的監控顯示：**</span><span class="sxs-lookup"><span data-stu-id="78306-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="78306-105">在同一時間按下列機碼： Windows 鍵 + Ctrl + Shift + b。這將會重新整理您的圖形驅動程式的通訊。</span><span class="sxs-lookup"><span data-stu-id="78306-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="78306-106">監視器將會短暫閃爍，和幾秒鐘之後再回來。</span><span class="sxs-lookup"><span data-stu-id="78306-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="78306-107">**疑難排解監視硬體：**</span><span class="sxs-lookup"><span data-stu-id="78306-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="78306-108">拔掉監視器]，並將它插回去連接您的電腦。</span><span class="sxs-lookup"><span data-stu-id="78306-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="78306-109">從您的電腦 （例如介面卡或停駐），中斷連線的任何非必要裝置。</span><span class="sxs-lookup"><span data-stu-id="78306-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="78306-110">**如果您最近在您的電腦上安裝更新，您可以回復顯示驅動程式：**</span><span class="sxs-lookup"><span data-stu-id="78306-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="78306-111">選取 [**開始**，輸入 **[裝置管理員]**，然後選取 [**裝置管理員**從結果。</span><span class="sxs-lookup"><span data-stu-id="78306-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="78306-112">展開 [**顯示卡**] 區段中，以滑鼠右鍵按一下 [顯示卡，and 選取**屬性**。</span><span class="sxs-lookup"><span data-stu-id="78306-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="78306-113">瀏覽至 [**驅動程式**] 索引標籤，然後選取 [**回復驅動程式**。</span><span class="sxs-lookup"><span data-stu-id="78306-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="78306-114">附註： 如果這無法使用，或是會變為灰色，選取 [**否**，將移至下一個步驟以下的選項。</span><span class="sxs-lookup"><span data-stu-id="78306-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="78306-115">您可能需要先重新啟動您的電腦，然後這些變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="78306-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="78306-116">**解除安裝並重新安裝驅動程式顯示：**</span><span class="sxs-lookup"><span data-stu-id="78306-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="78306-117">選取 [**開始**，輸入 **[裝置管理員]**，然後選取 [**裝置管理員**從結果。</span><span class="sxs-lookup"><span data-stu-id="78306-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="78306-118">展開 [**顯示卡**] 區段中，以滑鼠右鍵按一下 [顯示卡，and 選取**解除安裝的裝置**。</span><span class="sxs-lookup"><span data-stu-id="78306-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="78306-119">選取 [**刪除此裝置的驅動程式軟體**] 旁的方塊，然後選取 [**解除安裝**。</span><span class="sxs-lookup"><span data-stu-id="78306-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="78306-120">附註： 您可能會要求在此階段重新啟動電腦。</span><span class="sxs-lookup"><span data-stu-id="78306-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="78306-121">請確定您重新啟動之前記下的其餘的指示。</span><span class="sxs-lookup"><span data-stu-id="78306-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="78306-122">一次開啟 [裝置管理員]。</span><span class="sxs-lookup"><span data-stu-id="78306-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="78306-123">展開 [**顯示卡**] 區段中，以滑鼠右鍵按一下您的顯示卡，然後選取 [**更新驅動程式**。</span><span class="sxs-lookup"><span data-stu-id="78306-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="78306-124">選取 **[自動搜尋更新的驅動程式軟體**，然後按照安裝指示。</span><span class="sxs-lookup"><span data-stu-id="78306-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>