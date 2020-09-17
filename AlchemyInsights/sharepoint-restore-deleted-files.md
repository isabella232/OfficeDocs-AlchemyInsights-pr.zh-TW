---
title: 還原已刪除的檔案或資料夾
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797539"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="91460-102">還原已刪除的檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="91460-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="91460-103">SharePoint Online 在所有內容實際刪除之後，還會保留其備份額外 14 天。</span><span class="sxs-lookup"><span data-stu-id="91460-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="91460-104">如果透過回收站或檔案還原無法還原內容，系統管理員可以聯繫 Microsoft 支援部門，以在14天內的任何時間要求還原。</span><span class="sxs-lookup"><span data-stu-id="91460-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="91460-105">僅網站集合或子網站可以從備份進行還原，特定檔案、清單或媒體櫃則無法使用。</span><span class="sxs-lookup"><span data-stu-id="91460-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="91460-106">當您從 Sharepoint 刪除專案或網站時，並不會立即移除。</span><span class="sxs-lookup"><span data-stu-id="91460-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="91460-107">刪除的項目會在資源回收筒中一段時間。</span><span class="sxs-lookup"><span data-stu-id="91460-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="91460-108">在這段時間內，您可以將已刪除的項目還原到其原始位置。</span><span class="sxs-lookup"><span data-stu-id="91460-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="91460-109">如需詳細資訊，請瀏覽以下連結。</span><span class="sxs-lookup"><span data-stu-id="91460-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="91460-110">[還原 SharePoint 網站回收站中的專案](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b)。</span><span class="sxs-lookup"><span data-stu-id="91460-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="91460-111">還原 OneDrive 中已刪除的檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="91460-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="91460-112">還原已刪除的網站集合 (包括群組、通訊和其他網站) </span><span class="sxs-lookup"><span data-stu-id="91460-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="91460-113">還原已刪除的 OneDrive 網站</span><span class="sxs-lookup"><span data-stu-id="91460-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="91460-114">若為大量回收站動作，系統管理員可能會考慮使用 [Sharepoint ONLINE PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)。</span><span class="sxs-lookup"><span data-stu-id="91460-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="91460-115">**檔案還原功能**</span><span class="sxs-lookup"><span data-stu-id="91460-115">**Files Restore feature**</span></span>

<span data-ttu-id="91460-116">如果有大量 OneDrive 或 SharePoint 檔案遭到惡意程式碼的刪除、覆寫、損毀或感染，您可以使用 [檔案還原] 功能，將整個 OneDrive 或 SharePoint 文件庫還原至先前的時間。</span><span class="sxs-lookup"><span data-stu-id="91460-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="91460-117">還原 OneDrive 文件庫</span><span class="sxs-lookup"><span data-stu-id="91460-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="91460-118">還原文件庫</span><span class="sxs-lookup"><span data-stu-id="91460-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

