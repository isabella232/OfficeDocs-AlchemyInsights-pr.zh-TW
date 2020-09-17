---
title: 使用 TeamViewer 遠端管理 Intune 裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798439"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="fefd0-102">使用 TeamViewer 遠端管理 Intune 裝置</span><span class="sxs-lookup"><span data-stu-id="fefd0-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="fefd0-103">您可以使用 [TeamViewer](https://www.teamviewer.com/) 來遠端系統管理由 Intune 管理的裝置。</span><span class="sxs-lookup"><span data-stu-id="fefd0-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="fefd0-104">若要使用 TeamViewer 管理 Intune，請執行以下步驟：</span><span class="sxs-lookup"><span data-stu-id="fefd0-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="fefd0-105">首先從 TeamViewer 獲取認證以在 Intune 上設定TeamViewer 連接器。</span><span class="sxs-lookup"><span data-stu-id="fefd0-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="fefd0-106">這允許管理員在裝置底下的 TeamViewer 連接器 UI 中輸入認證，這是在 Intune 和 TeamViewer 服務之間建立連結的一次性操作。</span><span class="sxs-lookup"><span data-stu-id="fefd0-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="fefd0-107">**第 1 部分：使用遠端裝置啟動工作階段**</span><span class="sxs-lookup"><span data-stu-id="fefd0-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="fefd0-108">在 **[ 所有裝置 ]** 底下，選取您要啟動遠端工作階段的裝置。</span><span class="sxs-lookup"><span data-stu-id="fefd0-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="fefd0-109">從 **…更多**，選取**新遠端協助工作階段**。</span><span class="sxs-lookup"><span data-stu-id="fefd0-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="fefd0-110">選取 **[是]** 確認您要建立遠端工作階段。</span><span class="sxs-lookup"><span data-stu-id="fefd0-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="fefd0-111">在 TeamViewer 服務確認 [啟動新遠端工作階段] 要求後，您將在裝置的 [概觀] (或 [基本資訊]) 窗格的詳細資訊下看到 \*\*[啟動遠程協助] \*\*的選項。</span><span class="sxs-lookup"><span data-stu-id="fefd0-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="fefd0-112">選取 **[查看更多]** 展開窗格，並顯示 [遠端協助] 狀態。</span><span class="sxs-lookup"><span data-stu-id="fefd0-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="fefd0-113">選取 **[啟動遠端工作階段]**，在系統管理端啟動工作階段。</span><span class="sxs-lookup"><span data-stu-id="fefd0-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="fefd0-114">選擇下載 TeamViewer 二進位 (Windows)，然後選取 **[執行]**。</span><span class="sxs-lookup"><span data-stu-id="fefd0-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="fefd0-115">**附註** 您可以略過任何開啟到 TeamViewer 網站的網頁瀏覽器頁面。</span><span class="sxs-lookup"><span data-stu-id="fefd0-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="fefd0-116">確認 TeamViewer 應用程式在裝置上進行變更的要求 (僅限 Windows)。</span><span class="sxs-lookup"><span data-stu-id="fefd0-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="fefd0-117">TeamViewer 應用程式啟動並包含工作階段代碼，以驗證與遠端裝置的連線。</span><span class="sxs-lookup"><span data-stu-id="fefd0-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="fefd0-118">**第 2 部分：遠程工作階段的目標裝置上**</span><span class="sxs-lookup"><span data-stu-id="fefd0-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="fefd0-119">開啟 Intune 公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="fefd0-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="fefd0-120">尋找通知標識：「您的 IT 系統管理員正在請求遠端協助工作階段控制此裝置」，然後選取該通知。</span><span class="sxs-lookup"><span data-stu-id="fefd0-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="fefd0-121">選擇下載 TeamViewer 應用程式，或確認從 App Store 下載 TeamViewer 應用程式，然後選取 **[執行]**。</span><span class="sxs-lookup"><span data-stu-id="fefd0-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="fefd0-122">**附註** 您可以略過任何開啟到 TeamViewer 網站的網頁瀏覽器頁面。</span><span class="sxs-lookup"><span data-stu-id="fefd0-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="fefd0-123">確認 TeamViewer 應用程式在裝置上進行變更的要求 (僅限 Windows)。</span><span class="sxs-lookup"><span data-stu-id="fefd0-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="fefd0-124">TeamViewer 應用程式啟動並包含工作階段代碼，以驗證與遠端裝置的連線。</span><span class="sxs-lookup"><span data-stu-id="fefd0-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="fefd0-125">快顯詢問是否允許啟動工作階段。</span><span class="sxs-lookup"><span data-stu-id="fefd0-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="fefd0-126">**附註** TeamViewer 服務產生的工作階段代碼只能使用一次。</span><span class="sxs-lookup"><span data-stu-id="fefd0-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="fefd0-127">如果遺失連線，必須：</span><span class="sxs-lookup"><span data-stu-id="fefd0-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="fefd0-128">關閉遠端裝置和系統管理員工作站上的 TeamViewer 應用程式執行個體。</span><span class="sxs-lookup"><span data-stu-id="fefd0-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="fefd0-129">關閉遠端裝置上的公司入口網站。</span><span class="sxs-lookup"><span data-stu-id="fefd0-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="fefd0-130">從系統管理員入口網站開始新的「新遠端協助工作階段」。</span><span class="sxs-lookup"><span data-stu-id="fefd0-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="fefd0-131">重新開啟遠端裝置上的公司入口網站以接收新通知。</span><span class="sxs-lookup"><span data-stu-id="fefd0-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="fefd0-132">像之前一樣，在遠端裝置和系統管理員工作站上的下載和開啟 TeamViewer 應用程式。</span><span class="sxs-lookup"><span data-stu-id="fefd0-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>