---
title: Windows 10 中的啟動設定
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828143"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="a91c2-102">Windows 10 中的啟動設定</span><span class="sxs-lookup"><span data-stu-id="a91c2-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="a91c2-103">**變更啟動時自動執行的應用程式**</span><span class="sxs-lookup"><span data-stu-id="a91c2-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="a91c2-104">移至 [ [設定] > 應用程式 > 啟動](ms-settings:startupapps?activationSource=GetHelp)。</span><span class="sxs-lookup"><span data-stu-id="a91c2-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="a91c2-105">請確定開啟時您想要 **執行的任何** 應用程式已開啟。</span><span class="sxs-lookup"><span data-stu-id="a91c2-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="a91c2-106">**新增應用程式，以在啟動時自動執行**</span><span class="sxs-lookup"><span data-stu-id="a91c2-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="a91c2-107">按一下或點擊 [ **開始** ]，尋找您想要在啟動時執行的應用程式。</span><span class="sxs-lookup"><span data-stu-id="a91c2-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="a91c2-108">以滑鼠右鍵按一下應用程式，按一下 [ **其他**]，然後按一下 [ **開啟檔案位置**]。</span><span class="sxs-lookup"><span data-stu-id="a91c2-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="a91c2-109">這會開啟儲存應用程式快捷方式的位置。</span><span class="sxs-lookup"><span data-stu-id="a91c2-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="a91c2-110">如果開啟的檔案位置沒有任何選項，則表示應用程式無法在啟動時執行。</span><span class="sxs-lookup"><span data-stu-id="a91c2-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="a91c2-111">在檔案位置開啟時，按 **Windows 徽標鍵 + R**，輸入命令介面 **： startup**，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="a91c2-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="a91c2-112">這會開啟 [啟動] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="a91c2-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="a91c2-113">從檔案位置複製並貼上應用程式的快捷方式至 [啟動] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="a91c2-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="a91c2-114">**Advanced startup options (包括安全模式、UEFI 設定，以及從另一個裝置引導)**</span><span class="sxs-lookup"><span data-stu-id="a91c2-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="a91c2-115">儲存您的工作並關閉任何開啟的檔，因為這些步驟將會重新開機您的電腦。</span><span class="sxs-lookup"><span data-stu-id="a91c2-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="a91c2-116">移至 [ [設定] > 更新 & Security > Recovery](ms-settings:recovery?activationSource=GetHelp)。</span><span class="sxs-lookup"><span data-stu-id="a91c2-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="a91c2-117">在 [ **Advanced startup**] 底下，按一下 [ **立即重新開機**]。</span><span class="sxs-lookup"><span data-stu-id="a91c2-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="a91c2-118">在您的電腦重新開機至 [選擇選項] 畫面之後：</span><span class="sxs-lookup"><span data-stu-id="a91c2-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="a91c2-119">若要從 USB 磁片磁碟機等設備進行引導，請按一下 [ **使用裝置**]。</span><span class="sxs-lookup"><span data-stu-id="a91c2-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="a91c2-120">若要輸入 UEFI 設定 (有時稱為 BIOS 設定) ，請按一下 [ **疑難排解] > 高級選項 > UEFI 固件設定**。</span><span class="sxs-lookup"><span data-stu-id="a91c2-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="a91c2-121">若要輸入安全模式或變更 [advanced startup] 設定，請按一下 [ **疑難排解 > 高級選項] > 啟動設定**]，然後按一下 [ **重新開機**]。</span><span class="sxs-lookup"><span data-stu-id="a91c2-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="a91c2-122">您可能會要求您輸入 [BitLocker 復原金鑰](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)。</span><span class="sxs-lookup"><span data-stu-id="a91c2-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="a91c2-123">重新開機電腦之後，按一下您要使用的啟動設定。</span><span class="sxs-lookup"><span data-stu-id="a91c2-123">After your PC restarts again, click the startup setting you want to use.</span></span>