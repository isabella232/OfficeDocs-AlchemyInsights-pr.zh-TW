---
title: 檔案隨選
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791285"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="d487b-102">設定 [檔案隨選]</span><span class="sxs-lookup"><span data-stu-id="d487b-102">Configure Files On-Demand</span></span>

<span data-ttu-id="d487b-103">[OneDrive 檔案隨選] 需要 [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040)（版本 1709 或更新版本）或 Windows Server 2019 及 OneDrive 組建 17.3.7064.1005 或更新版本。</span><span class="sxs-lookup"><span data-stu-id="d487b-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="d487b-104">OneDrive [檔案隨選] 能協助您存取 OneDrive 中的所有檔案，而不必全部下載並占用您裝置上的儲存空間。</span><span class="sxs-lookup"><span data-stu-id="d487b-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="d487b-105">若要在您的電腦上設定 [檔案隨選]：</span><span class="sxs-lookup"><span data-stu-id="d487b-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="d487b-106">選取 Windows 工作列通知區域中的藍色 **OneDrive** 雲朵圖示。</span><span class="sxs-lookup"><span data-stu-id="d487b-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="d487b-107">選取 **[說明與設定]** 齒輪圖示 > **[設定]** 。</span><span class="sxs-lookup"><span data-stu-id="d487b-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="d487b-108">在 **[設定]** 索引標籤上，選取 **[節省空間並在使用的同時下載檔案]** 方塊。</span><span class="sxs-lookup"><span data-stu-id="d487b-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="d487b-109">您也可以使用登錄設定 [檔案隨選]。</span><span class="sxs-lookup"><span data-stu-id="d487b-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="d487b-110">如果停用此設定，Windows 10 使用者會與 Windows 舊版使用者有相同的同步處理行為，且將無法開啟檔案隨選。</span><span class="sxs-lookup"><span data-stu-id="d487b-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="d487b-111">如果不設定此設定，使用者可以開啟或關閉檔案檔案隨選。</span><span class="sxs-lookup"><span data-stu-id="d487b-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="d487b-112">啟用此原則會將下列登錄機碼值設為 1。</span><span class="sxs-lookup"><span data-stu-id="d487b-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="d487b-113">停用此原則會將下列登錄機碼值設為 0。</span><span class="sxs-lookup"><span data-stu-id="d487b-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="d487b-114">若您無法在 [設定] 中看見 [檔案隨選]，請確認服務 "Windows Cloud Files Filter Driver" 的啟動類型設定為 2 (AUTO_START)。</span><span class="sxs-lookup"><span data-stu-id="d487b-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="d487b-115">啟用此功能會將下列登錄機碼值設為 2。</span><span class="sxs-lookup"><span data-stu-id="d487b-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`