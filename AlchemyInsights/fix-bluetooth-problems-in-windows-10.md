---
title: 修正 Windows 10 中藍牙問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001475"
- "3506"
ms.openlocfilehash: 94dda7a42632f57ce3aef5f467b87df1033b8d49
ms.sourcegitcommit: 9a35768444824cde9e192f1d9daafc9157437244
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268568"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="5d2c3-102">修正 Windows 10 中藍牙問題</span><span class="sxs-lookup"><span data-stu-id="5d2c3-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="5d2c3-103">如果藍牙圖示遺漏或藍芽無法開啟或關閉，您可能想要執行藍芽疑難排解員。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="5d2c3-104">[開啟 [疑難排解] 設定](ms-settings:troubleshoot)，請按一下下**找出並修正其他問題**的**藍牙**，按一下 [**執行疑難排解員**。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="5d2c3-105">如果您沒有看到 [藍牙] 圖示，但藍芽就會出現在 [裝置管理員] 中：</span><span class="sxs-lookup"><span data-stu-id="5d2c3-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="5d2c3-106">在 [裝置管理員] 中，按一下 [**藍牙**]。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="5d2c3-107">按下及保留 （或以滑鼠右鍵按一下） [藍牙配接器名稱，然後按一下 [**解除安裝的裝置**。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="5d2c3-108">關閉您的 Windows 裝置、 等候幾秒，然後再將它重新開啟。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="5d2c3-109">Windows 會嘗試重新安裝驅動程式。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="5d2c3-110">如果您最近安裝 Windows 10 更新或升級至 Windows 10 時，您可能想要檢查的驅動程式更新：</span><span class="sxs-lookup"><span data-stu-id="5d2c3-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="5d2c3-111">在 [裝置管理員] 中，按一下 [**藍牙**，，，然後按一下 [藍牙配接器名稱 （其中可能包含 「 選項 」 這個字）。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="5d2c3-112">按下及保留 （或以滑鼠右鍵按一下） [藍牙介面卡，然後按一下 [**更新驅動程式** > **自動搜尋更新的驅動程式軟體]**。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="5d2c3-113">請依照下列步驟，然後按一下 [**關閉**]。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="5d2c3-114">如果 Windows 找不到新的藍芽驅動程式，請造訪電腦製造商的網站，並從該處下載最新的藍芽驅動程式。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="5d2c3-115">在下載之後，按一下 [**更新驅動程式** > **瀏覽電腦上的驅動程式軟體** > 驅動程式檔案的所在位置的 [**瀏覽**儲存 >**確定** > **下一步**，並遵循步驟來安裝。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="5d2c3-116">安裝更新的驅動程式之後, 重新啟動電腦，並檢查是否會修正連線問題。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="5d2c3-117">如需如何將藍牙問題疑難排解的詳細資訊，請參閱完整的文章，[在 Windows 10 中的修正藍牙問題](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems)。</span><span class="sxs-lookup"><span data-stu-id="5d2c3-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
