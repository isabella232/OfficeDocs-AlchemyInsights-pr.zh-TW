---
title: 檔案隨選
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406552"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="8f647-102">設定 [檔案隨選]</span><span class="sxs-lookup"><span data-stu-id="8f647-102">Configure Files On-Demand</span></span>

<span data-ttu-id="8f647-103">OneDrive [檔案隨選] 能協助您存取 OneDrive 中的所有檔案，而不必全部下載並占用您裝置上的儲存空間。</span><span class="sxs-lookup"><span data-stu-id="8f647-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="8f647-104">若要在您的電腦上設定 [檔案隨選]：</span><span class="sxs-lookup"><span data-stu-id="8f647-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="8f647-105">選取 Windows 工作列通知區域中的藍色 **OneDrive** 雲朵圖示。</span><span class="sxs-lookup"><span data-stu-id="8f647-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="8f647-106">選取 **[說明與設定]** 齒輪圖示 > **[設定]**。</span><span class="sxs-lookup"><span data-stu-id="8f647-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="8f647-107">在 **[設定]** 索引標籤上，選取 **[節省空間並在使用的同時下載檔案]** 方塊。</span><span class="sxs-lookup"><span data-stu-id="8f647-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="8f647-108">您也可以使用登錄設定 [檔案隨選]。</span><span class="sxs-lookup"><span data-stu-id="8f647-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="8f647-109">如果停用此設定，Windows 10 使用者會與 Windows 舊版使用者有相同的同步處理行為，且將無法開啟檔案隨選。</span><span class="sxs-lookup"><span data-stu-id="8f647-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="8f647-110">如果不設定此設定，使用者可以開啟或關閉檔案檔案隨選。</span><span class="sxs-lookup"><span data-stu-id="8f647-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="8f647-111">啟用此原則會將下列登錄機碼值設為 1。</span><span class="sxs-lookup"><span data-stu-id="8f647-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="8f647-112">停用此原則會將下列登錄機碼值設為 0。</span><span class="sxs-lookup"><span data-stu-id="8f647-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="8f647-113">若您無法在 [設定] 中看見 [檔案隨選]，請確認服務 "Windows Cloud Files Filter Driver" 的啟動類型設定為 2 (AUTO_START)。</span><span class="sxs-lookup"><span data-stu-id="8f647-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="8f647-114">啟用此功能會將下列登錄機碼值設為 2。</span><span class="sxs-lookup"><span data-stu-id="8f647-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`