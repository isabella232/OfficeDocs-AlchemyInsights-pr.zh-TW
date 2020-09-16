---
title: 疑難排解 Windows 10 中的音訊問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750298"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="b9c98-102">疑難排解 Windows 10 中的音訊問題</span><span class="sxs-lookup"><span data-stu-id="b9c98-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="b9c98-103">**執行音訊疑難排解程式**</span><span class="sxs-lookup"><span data-stu-id="b9c98-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="b9c98-104">開啟 [疑難排解設定](ms-settings:troubleshoot)。</span><span class="sxs-lookup"><span data-stu-id="b9c98-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="b9c98-105">選取 [**播放音訊**]  >  **執行疑難排解**程式。</span><span class="sxs-lookup"><span data-stu-id="b9c98-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="b9c98-106">**設定預設裝置**</span><span class="sxs-lookup"><span data-stu-id="b9c98-106">**Set the default device**</span></span>

<span data-ttu-id="b9c98-107">如果您是使用 USB 或 HDMI 連接至音訊裝置，您可能需要將該裝置設為預設值：</span><span class="sxs-lookup"><span data-stu-id="b9c98-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="b9c98-108">開啟 [**開始**  >  **聲音**]，然後從結果清單中選取 [**聲音**] 或 [**變更系統聲音**]。</span><span class="sxs-lookup"><span data-stu-id="b9c98-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="b9c98-109">在 [ **播放** ] 索引標籤上，選取裝置，選取 [ **設定預設**]，然後選取 **[確定**]。</span><span class="sxs-lookup"><span data-stu-id="b9c98-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="b9c98-110">**檢查纜線、成交量、喇叭和耳機**</span><span class="sxs-lookup"><span data-stu-id="b9c98-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="b9c98-111">檢查您的喇叭和耳機連接是否有鬆動的電纜，並確定它們已連接至正確的插座。</span><span class="sxs-lookup"><span data-stu-id="b9c98-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="b9c98-112">檢查電源和音量層級，然後嘗試開啟所有音量控制。</span><span class="sxs-lookup"><span data-stu-id="b9c98-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="b9c98-113">有些揚聲器和應用程式有自己的音量控制;您可能需要全部檢查，以確定它們是正確的層級。</span><span class="sxs-lookup"><span data-stu-id="b9c98-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="b9c98-114">請嘗試使用不同的 USB 埠進行連接。</span><span class="sxs-lookup"><span data-stu-id="b9c98-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="b9c98-115">**附注**：請記住，當插入耳機時，您的揚聲器可能無法運作。</span><span class="sxs-lookup"><span data-stu-id="b9c98-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="b9c98-116">**檢查裝置管理員**</span><span class="sxs-lookup"><span data-stu-id="b9c98-116">**Check Device Manager**</span></span>

<span data-ttu-id="b9c98-117">若要確定驅動程式是最新的：</span><span class="sxs-lookup"><span data-stu-id="b9c98-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="b9c98-118">選取 [ **開始**]，輸入 [ **裝置管理員**]，然後從結果清單中選取 [ **裝置管理員** ]。</span><span class="sxs-lookup"><span data-stu-id="b9c98-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="b9c98-119">在 [ **聲音、影片及遊戲控制器**] 底下，選取您的音效卡，開啟它，選取 [ **驅動程式** ] 索引標籤，然後選取 [ **更新驅動程式**]。</span><span class="sxs-lookup"><span data-stu-id="b9c98-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="b9c98-120">**附注**：如果 Windows 找不到新的驅動程式，請在設備製造商網站上尋找一個，然後依照指示執行。</span><span class="sxs-lookup"><span data-stu-id="b9c98-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="b9c98-121">**重新安裝驅動程式**</span><span class="sxs-lookup"><span data-stu-id="b9c98-121">**Reinstall the driver**</span></span>

<span data-ttu-id="b9c98-122">如果您無法透過裝置管理員更新或在製造商的網站上尋找新的驅動程式，請嘗試下列步驟：</span><span class="sxs-lookup"><span data-stu-id="b9c98-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="b9c98-123">在 [裝置管理員] 中，以滑鼠右鍵按一下 (或長按) 音訊驅動程式，然後選取 [ **卸載**]。</span><span class="sxs-lookup"><span data-stu-id="b9c98-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="b9c98-124">重新開機裝置，Windows 將會嘗試重新安裝驅動程式。</span><span class="sxs-lookup"><span data-stu-id="b9c98-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="b9c98-125">若重新安裝驅動程式無法運作，請嘗試使用 Windows 隨附的一般音訊驅動程式。</span><span class="sxs-lookup"><span data-stu-id="b9c98-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="b9c98-126">在 [裝置管理員] 中，以滑鼠右鍵按一下 (，或長按) 音訊驅動程式 >**更新驅動程式軟體**  >  **流覽 [我的電腦] 以取得驅動程式軟體**  >  。請**從 [我的電腦] 的裝置驅動程式清單**中選取 [ **High Definition audio 裝置**]，選取 **[下一步]**，然後依照指示安裝。</span><span class="sxs-lookup"><span data-stu-id="b9c98-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
