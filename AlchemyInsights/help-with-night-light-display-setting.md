---
title: 夜間光線顯示設定說明
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123042"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="a68af-102">夜間光線顯示設定說明</span><span class="sxs-lookup"><span data-stu-id="a68af-102">Help with the night light display setting</span></span>

<span data-ttu-id="a68af-103">若要深入了解夜間顯示設定，請參閱 [在 Windows 10 中設定顯示器於夜間使用](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136)。</span><span class="sxs-lookup"><span data-stu-id="a68af-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="a68af-104">如果夜間光線選項在 [設定] 中顯示為灰色，請檢查您的顯示器驅動程式：</span><span class="sxs-lookup"><span data-stu-id="a68af-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="a68af-105">按一下工作列上的搜尋方塊，然後輸入 **[裝置管理員]**，然後在搜尋結果中選取 **[裝置管理員]**。</span><span class="sxs-lookup"><span data-stu-id="a68af-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="a68af-106">展開 **[顯示卡]**。</span><span class="sxs-lookup"><span data-stu-id="a68af-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="a68af-107">很抱歉，如果您的裝置使用 DisplayLink 驅動程式或基本顯示器驅動程式，夜間光線功能將不可用。</span><span class="sxs-lookup"><span data-stu-id="a68af-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="a68af-108">夜間光線功能會使用最新的圖形技術，因此您可能需要更新顯示器驅動程式：</span><span class="sxs-lookup"><span data-stu-id="a68af-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="a68af-109">若要檢查更新，請前往 **[開始]** > **[設定]** > **[更新與安全性]** > **[Windows Update]** > **[檢查更新]**。</span><span class="sxs-lookup"><span data-stu-id="a68af-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="a68af-110">或</span><span class="sxs-lookup"><span data-stu-id="a68af-110">OR</span></span>

- <span data-ttu-id="a68af-111">請瀏覽硬體製造商的支援網站，以手動下載並安裝最新的顯示器驅動程式。</span><span class="sxs-lookup"><span data-stu-id="a68af-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="a68af-112">重設登錄中的夜間光線</span><span class="sxs-lookup"><span data-stu-id="a68af-112">Reset night light in the registry</span></span>

<span data-ttu-id="a68af-113">如果更新顯示器驅動程式未起作用，您可能需要在登錄中重設夜間光線。</span><span class="sxs-lookup"><span data-stu-id="a68af-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="a68af-114">**注意：** 只建議進階使用者使用這個疑難排解步驟。</span><span class="sxs-lookup"><span data-stu-id="a68af-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="a68af-115">如果未能正確修改登錄，可能會發生嚴重的問題。</span><span class="sxs-lookup"><span data-stu-id="a68af-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="a68af-116">若要增添一層防護，請先備份登錄再進行修改。如此一來，如果發生問題，您便能加以還原。</span><span class="sxs-lookup"><span data-stu-id="a68af-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="a68af-117">在搜尋方塊中，輸入 **regedit**，然後在搜尋結果中選取 **[登錄編輯程式]**。</span><span class="sxs-lookup"><span data-stu-id="a68af-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="a68af-118">移至下列登錄機碼：</span><span class="sxs-lookup"><span data-stu-id="a68af-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="a68af-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="a68af-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="a68af-120">匯出然後刪除下列子機碼：$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="a68af-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="a68af-121">匯出然後刪除下列子機碼：$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="a68af-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="a68af-122">重新啟動 Windows，並驗證夜間光線選項是否可用。</span><span class="sxs-lookup"><span data-stu-id="a68af-122">Restart Windows and verify if the night light options are available.</span></span>


