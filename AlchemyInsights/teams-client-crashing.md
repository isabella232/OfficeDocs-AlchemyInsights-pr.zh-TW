---
title: Teams 用戶端當機？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030540"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="17612-102">Teams 用戶端當機？</span><span class="sxs-lookup"><span data-stu-id="17612-102">Teams client crashing?</span></span>

<span data-ttu-id="17612-103">如果您的 Teams 用戶端當機，請嘗試下列操作：</span><span class="sxs-lookup"><span data-stu-id="17612-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="17612-104">如果您使用的是 Teams 傳統型應用程式，請[確定應用程式已完全更新](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)。</span><span class="sxs-lookup"><span data-stu-id="17612-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="17612-105">請確定所有 [Office 365 URL 和位址範圍](https://docs.microsoft.com/microsoftteams/connectivity-issues)皆可存取。</span><span class="sxs-lookup"><span data-stu-id="17612-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="17612-106">使用您的系統管理員帳戶登入，並檢查您的[服務健康情況儀表板](https://docs.microsoft.com/office365/enterprise/view-service-health) (部分機器翻譯)，確認沒有中斷或服務降級。</span><span class="sxs-lookup"><span data-stu-id="17612-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="17612-107">最後，您可以嘗試清除 Teams 用戶端快取：</span><span class="sxs-lookup"><span data-stu-id="17612-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="17612-108">完全關閉 Microsoft Teams 桌面用戶端。</span><span class="sxs-lookup"><span data-stu-id="17612-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="17612-109">您可以在圖示匣中，以滑鼠右鍵按一下 [Teams]\*\*\*\*，然後按一下 [結束]\*\*\*\* 或執行 [工作管理員] 並完全終止程序。</span><span class="sxs-lookup"><span data-stu-id="17612-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="17612-110">移至 [檔案總管]，然後輸入 %appdata%\Microsoft\teams。</span><span class="sxs-lookup"><span data-stu-id="17612-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="17612-111">在目錄中，您會看到下列幾個資料夾：</span><span class="sxs-lookup"><span data-stu-id="17612-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="17612-112">在 [應用程式快取]\*\*\*\* 內，移至 [快取]，並刪除 [快取] 位置中的任何檔案：%appdata%\Microsoft\teams\application cache\cache。</span><span class="sxs-lookup"><span data-stu-id="17612-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="17612-113">在 [Blob_storage]\*\*\*\* 內，刪除所有檔案：%appdata%\Microsoft\teams\blob_storage。</span><span class="sxs-lookup"><span data-stu-id="17612-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="17612-114">在 [快取]\*\*\*\* 內，刪除所有檔案：%appdata%\Microsoft\teams\Cache。</span><span class="sxs-lookup"><span data-stu-id="17612-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="17612-115">在 [資料庫]\*\*\*\* 內，刪除所有檔案：%appdata%\Microsoft\teams\databases。</span><span class="sxs-lookup"><span data-stu-id="17612-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="17612-116">在 [GPUCache]\*\*\*\* 內，刪除所有檔案：%appdata%\Microsoft\teams\GPUcache。</span><span class="sxs-lookup"><span data-stu-id="17612-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="17612-117">在 [IndexedDB]\*\*\*\* 內，刪除 .db 檔案：%appdata%\Microsoft\teams\IndexedDB。</span><span class="sxs-lookup"><span data-stu-id="17612-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="17612-118">在 [本機儲存體]\*\*\*\* 內，刪除所有檔案：%appdata%\Microsoft\teams\Local Storage。</span><span class="sxs-lookup"><span data-stu-id="17612-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="17612-119">最後，在 [tmp]\*\*\*\* 內，刪除任何檔案：%appdata%\Microsoft\teams\tmp。</span><span class="sxs-lookup"><span data-stu-id="17612-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="17612-120">重新啟動您的 Teams 用戶端。</span><span class="sxs-lookup"><span data-stu-id="17612-120">Restart your Teams client.</span></span>
