---
title: 在 Windows 10 中釋放磁碟機空間
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505347"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a8f77-102">在 Windows 10 中釋放磁碟機空間</span><span class="sxs-lookup"><span data-stu-id="a8f77-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a8f77-103">以下是在 Windows 10 中釋放磁碟機空間的兩種選項：</span><span class="sxs-lookup"><span data-stu-id="a8f77-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a8f77-104">在 Windows 10 中釋放磁碟機空間。</span><span class="sxs-lookup"><span data-stu-id="a8f77-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a8f77-105">使用外部存放裝置釋放 Windows 10 更新的空間。</span><span class="sxs-lookup"><span data-stu-id="a8f77-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a8f77-106">如果使用 [磁碟清理] 後，磁碟空間仍然不足，您的 Temp 資料夾可能快速填滿 Microsoft Store 所使用的應用程式 (.appx) 檔案。</span><span class="sxs-lookup"><span data-stu-id="a8f77-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a8f77-107">若要修正此問題，請重設 Microsoft Store、清除 Microsoft Store 快取，然後執行 Windows Update 疑難排解員。</span><span class="sxs-lookup"><span data-stu-id="a8f77-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a8f77-108">執行這些步驟之前，請確定 Microsoft Store 已關閉。</span><span class="sxs-lookup"><span data-stu-id="a8f77-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a8f77-109">**步驟 1：重設 Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="a8f77-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a8f77-110">**請注意** 這會永久刪除裝置上的應用程式資料，包括您的喜好設定和登入詳細資料。</span><span class="sxs-lookup"><span data-stu-id="a8f77-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a8f77-111">選取 **[開始]** > **[設定]** > **[應用程式]** > **[應用程式與功能]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a8f77-112">在應用程式清單中，尋找並選取 Microsoft Store。</span><span class="sxs-lookup"><span data-stu-id="a8f77-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a8f77-113">選取 **[進階選項]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a8f77-114">向下捲動並選取 **[重設]**，然後選取 **[確認重設]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a8f77-115">**步驟 2：清除 Microsoft Store 快取**</span><span class="sxs-lookup"><span data-stu-id="a8f77-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a8f77-116">按下 Windows 標誌鍵+R，開啟 [執行] 對話方塊。</span><span class="sxs-lookup"><span data-stu-id="a8f77-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a8f77-117">輸入 wsreset.exe，並選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a8f77-118">空白命令提示視窗會隨即開啟。</span><span class="sxs-lookup"><span data-stu-id="a8f77-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a8f77-119">約 10 秒之後，視窗關閉，Windows Store 會自動開啟。</span><span class="sxs-lookup"><span data-stu-id="a8f77-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a8f77-120">**步驟 3：重設 Windows Update**</span><span class="sxs-lookup"><span data-stu-id="a8f77-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a8f77-121">選取 **[開始]** > **[設定]** > **[更新與安全性]** > **[疑難排解]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a8f77-122">向下捲動並選取 **[Windows Update]**，然後選取 **[執行疑難排解員]**。</span><span class="sxs-lookup"><span data-stu-id="a8f77-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a8f77-123">將電腦重新開機，並檢查您是否仍遇到問題。</span><span class="sxs-lookup"><span data-stu-id="a8f77-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

