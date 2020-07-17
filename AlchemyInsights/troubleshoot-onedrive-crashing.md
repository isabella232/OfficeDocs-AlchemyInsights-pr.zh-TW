---
title: 疑難排解 OneDrive 當機問題
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/15/2020
ms.locfileid: "44735386"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="9385d-102">疑難排解 OneDrive 當機問題</span><span class="sxs-lookup"><span data-stu-id="9385d-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="9385d-103">如果 OneDrive 重複當機，請嘗試下列疑難排解步驟：</span><span class="sxs-lookup"><span data-stu-id="9385d-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="9385d-104">**確定是否設定登錄機碼：**</span><span class="sxs-lookup"><span data-stu-id="9385d-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="9385d-105">使用 [登錄編輯程式]，並瀏覽至 HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="9385d-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="9385d-106">如果有 DisableFileSyncNGSC 且設定為 1，請開啟機碼並將值變更為 0。</span><span class="sxs-lookup"><span data-stu-id="9385d-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="9385d-107">移至 [開始] 手動啟動 OneDrive</span><span class="sxs-lookup"><span data-stu-id="9385d-107">Manually launch OneDrive by going to Start</span></span> ![按 Windows 鍵](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="9385d-109">，在 [搜尋] 方塊中輸入 OneDrive，然後按一下 OneDrive 傳統型應用程式。</span><span class="sxs-lookup"><span data-stu-id="9385d-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="9385d-110">**重設 OneDrive：**</span><span class="sxs-lookup"><span data-stu-id="9385d-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="9385d-111">附註：</span><span class="sxs-lookup"><span data-stu-id="9385d-111">Notes:</span></span>

- <span data-ttu-id="9385d-112">重設 OneDrive 會中斷所有現有的同步處理連線 (如果有設定的話，包含您個人的 OneDrive)。</span><span class="sxs-lookup"><span data-stu-id="9385d-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="9385d-113">重設電腦上的 OneDrive 並不會遺失檔案或資料。</span><span class="sxs-lookup"><span data-stu-id="9385d-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="9385d-114">**重設 OneDrive：**</span><span class="sxs-lookup"><span data-stu-id="9385d-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="9385d-115">按下 Windows 鍵和 R 開啟 [執行] 對話方塊。</span><span class="sxs-lookup"><span data-stu-id="9385d-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="9385d-116">輸入 %localappdata%\Microsoft\OneDrive\onedrive.exe /reset，然後按下 [確定]。</span><span class="sxs-lookup"><span data-stu-id="9385d-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="9385d-117">會短暫出現一個 [命令] 視窗。</span><span class="sxs-lookup"><span data-stu-id="9385d-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="9385d-118">移至 [開始] 手動啟動 OneDrive</span><span class="sxs-lookup"><span data-stu-id="9385d-118">Manually launch OneDrive by going to Start</span></span> ![按 Windows 鍵](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="9385d-120">，在 [搜尋] 方塊中輸入 OneDrive，然後按一下 OneDrive 傳統型應用程式。</span><span class="sxs-lookup"><span data-stu-id="9385d-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="9385d-121">附註：</span><span class="sxs-lookup"><span data-stu-id="9385d-121">Notes:</span></span>

- <span data-ttu-id="9385d-122">如果您在重設前已選擇只同步處理部分的資料夾，您會需要在同步處理完成之後再次設定。</span><span class="sxs-lookup"><span data-stu-id="9385d-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="9385d-123">如需詳細資訊，請閱讀 [選擇要同步處理到電腦的 OneDrive 資料夾](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) 。</span><span class="sxs-lookup"><span data-stu-id="9385d-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="9385d-124">您需要為個人 OneDrive 和商務用 OneDrive 完成此步驟。</span><span class="sxs-lookup"><span data-stu-id="9385d-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>