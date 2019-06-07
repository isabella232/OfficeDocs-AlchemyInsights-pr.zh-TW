---
title: 還原已刪除的檔案或資料夾
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: 1672f425719597b93b8ef05865797714c3b19e42
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758897"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="e839b-102">還原已刪除的檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="e839b-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="e839b-103">SharePoint Online 會保留所有內容的備份實際刪除超過 14 其他天。</span><span class="sxs-lookup"><span data-stu-id="e839b-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="e839b-104">如果內容無法還原透過資源回收筒或檔案還原，系統管理員可以連絡 Microsoft 支援服務要求還原 14 天的期間內的任何時間。</span><span class="sxs-lookup"><span data-stu-id="e839b-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="e839b-105">網站集合或子網站，不適用於特定的檔案、 清單或文件庫，才可完成從備份還原。</span><span class="sxs-lookup"><span data-stu-id="e839b-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="e839b-106">當您從 Sharepoint 刪除項目或網站時，就無法立即被刪除。</span><span class="sxs-lookup"><span data-stu-id="e839b-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="e839b-107">已刪除的項目移至資源回收筒一段時間。</span><span class="sxs-lookup"><span data-stu-id="e839b-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="e839b-108">在這段時間，您可以還原已刪除的項目至其原始位置。</span><span class="sxs-lookup"><span data-stu-id="e839b-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="e839b-109">如需詳細資訊，請瀏覽下列連結。</span><span class="sxs-lookup"><span data-stu-id="e839b-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="e839b-110">[在 SharePoint 網站資源回收筒還原項目](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US)。</span><span class="sxs-lookup"><span data-stu-id="e839b-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="e839b-111">還原已刪除的檔案或 OneDrive 中的資料夾</span><span class="sxs-lookup"><span data-stu-id="e839b-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="e839b-112">還原已刪除的網站集合 （包括群組、 通訊以及其他網站）</span><span class="sxs-lookup"><span data-stu-id="e839b-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="e839b-113">還原已刪除的 OneDrive 網站</span><span class="sxs-lookup"><span data-stu-id="e839b-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="e839b-114">大量資源回收筒] 動作，系統管理員可能會考慮使用[Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)。</span><span class="sxs-lookup"><span data-stu-id="e839b-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="e839b-115">**檔案還原功能**</span><span class="sxs-lookup"><span data-stu-id="e839b-115">**Files Restore feature**</span></span>

<span data-ttu-id="e839b-116">如果您的 OneDrive 或 SharePoint 檔案大量取得刪除、 覆寫、 損毀，或感染惡意程式碼，您可以還原您整個 OneDrive 或 SharePoint 文件庫至前一次使用的檔案還原功能。</span><span class="sxs-lookup"><span data-stu-id="e839b-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="e839b-117">還原 OneDrive 文件庫</span><span class="sxs-lookup"><span data-stu-id="e839b-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="e839b-118">還原的文件庫</span><span class="sxs-lookup"><span data-stu-id="e839b-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

