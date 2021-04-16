---
title: 修正 Windows 10 中的藍牙問題
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812923"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="10094-102">修正 Windows 10 中的藍牙問題</span><span class="sxs-lookup"><span data-stu-id="10094-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="10094-103">如果藍牙圖示遺失或無法開啟或關閉藍牙，您可能想要執行藍牙疑難排解。</span><span class="sxs-lookup"><span data-stu-id="10094-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="10094-104">[開啟疑難排解設定](ms-settings:troubleshoot)、按一下 [ **藍牙** ] 下方的 [ **尋找並修正其他問題**]，按一下 **[執行疑難排解**]。</span><span class="sxs-lookup"><span data-stu-id="10094-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="10094-105">如果您未看到藍牙圖示，但是藍牙會出現在裝置管理器中：</span><span class="sxs-lookup"><span data-stu-id="10094-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="10094-106">在 [裝置管理員] 中，按一下 [ **藍牙**]。</span><span class="sxs-lookup"><span data-stu-id="10094-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="10094-107">長按 (或以滑鼠右鍵按一下藍牙配接器名稱) ，然後按一下 [ **卸載裝置**]。</span><span class="sxs-lookup"><span data-stu-id="10094-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="10094-108">請關閉 Windows 裝置，等候幾秒，然後再將它重新開啟。</span><span class="sxs-lookup"><span data-stu-id="10094-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="10094-109">Windows 會嘗試重新安裝驅動程式。</span><span class="sxs-lookup"><span data-stu-id="10094-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="10094-110">如果您最近安裝了 Windows 10 更新或升級至 Windows 10，您可能需要檢查驅動程式更新：</span><span class="sxs-lookup"><span data-stu-id="10094-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="10094-111">在 [裝置管理員] 中，按一下 [ **藍牙**]，然後按一下可能包含 "收音機" 一字 ") 的藍牙介面卡名稱 (。</span><span class="sxs-lookup"><span data-stu-id="10094-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="10094-112">長按 (或以滑鼠右鍵按一下藍牙配接器) ，然後按一下 [自動 **更新驅動程式**  >  **搜尋] 以更新的驅動程式軟體**。</span><span class="sxs-lookup"><span data-stu-id="10094-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="10094-113">遵循步驟，然後按一下 [ **關閉**]。</span><span class="sxs-lookup"><span data-stu-id="10094-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="10094-114">如果 Windows 找不到新的藍牙驅動程式，請造訪電腦製造商的網站，並從那裡下載最新的藍牙驅動程式。</span><span class="sxs-lookup"><span data-stu-id="10094-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="10094-115">下載後，請按一下 [**更新驅動** 程式  >  **] 流覽「我的電腦以取得驅動程式軟體**」  >  **流覽** 存放驅動程式檔案所在的位置。 >**確定**  >  **] 下一步**，然後依照安裝的步驟進行安裝。</span><span class="sxs-lookup"><span data-stu-id="10094-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="10094-116">安裝更新的驅動程式後，請重新開機電腦，然後檢查是否修正連線問題。</span><span class="sxs-lookup"><span data-stu-id="10094-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="10094-117">如需如何疑難排解藍牙問題的詳細資訊，請參閱完整的文章， [修正 Windows 10 中的藍牙問題](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)。</span><span class="sxs-lookup"><span data-stu-id="10094-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
