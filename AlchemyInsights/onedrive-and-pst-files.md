---
title: OneDrive 和 .pst 檔案
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
- "6002"
- "9003081"
ms.openlocfilehash: 16dfc5b39be7967a6de7967edee28bc7f08d216b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47673236"
---
# <a name="onedrive-and-pst-files"></a><span data-ttu-id="05f29-102">OneDrive 和 .pst 檔案</span><span class="sxs-lookup"><span data-stu-id="05f29-102">OneDrive and .pst files</span></span> 

<span data-ttu-id="05f29-103">OneDrive 支援 Outlook .pst 檔案，不過為減少網路流量它們的同步處理頻率比其他檔案類型還要低。</span><span class="sxs-lookup"><span data-stu-id="05f29-103">OneDrive supports Outlook .pst files, however, they're synced less frequently compared to other file types to reduce network traffic.</span></span> <span data-ttu-id="05f29-104">若要避免 OneDrive 同步處理應用程式上傳 .pst 檔案，請參閱 [封鎖特定檔案類型的同步處理](https://docs.microsoft.com/onedrive/block-file-types)。</span><span class="sxs-lookup"><span data-stu-id="05f29-104">To prevent the OneDrive sync app from uploading .pst files, see [Block syncing of specific file types](https://docs.microsoft.com/onedrive/block-file-types).</span></span> 

<span data-ttu-id="05f29-105">若要將 .pst 檔案移至 OneDrive，請參閱 [如何從 OneDrive 中移除 Outlook .pst 資料檔](https://support.microsoft.com/office/how-to-remove-an-outlook-pst-data-file-from-onedrive-b6b9e522-59bd-40f7-949f-168d0aa9b38e)。</span><span class="sxs-lookup"><span data-stu-id="05f29-105">To move .pst files out of OneDrive, see [How to remove an Outlook .pst data file from OneDrive](https://support.microsoft.com/office/how-to-remove-an-outlook-pst-data-file-from-onedrive-b6b9e522-59bd-40f7-949f-168d0aa9b38e).</span></span> 

<span data-ttu-id="05f29-106">如果使用者在不使用群組原則的情況下，手動啟用 PC 資料夾備份，則若他們已知的資料夾中有 .pst 檔案的話，會發生錯誤。</span><span class="sxs-lookup"><span data-stu-id="05f29-106">If users enable PC folder backup manually without the group policy, an error occurs if they have a .pst file in one of their known folders.</span></span>

<span data-ttu-id="05f29-107">如果您使用的是公司或學校的 OneDrive，某些檔案類型可能會受到組織 SharePoint 網站系統管理員的封鎖。</span><span class="sxs-lookup"><span data-stu-id="05f29-107">If you use OneDrive for work or school, some file types might be blocked by the organization SharePoint site admin.</span></span>