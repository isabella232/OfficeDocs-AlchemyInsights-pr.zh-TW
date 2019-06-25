---
title: 疑難排解錯誤 404, 找不到檔案
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 1b15444c-367b-4523-8e08-1c77bbea7524
ms.openlocfilehash: 045c29520ec60f9f093d3c9f129213213826466e
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757669"
---
# <a name="troubleshoot-error-404-file-not-found"></a><span data-ttu-id="06e08-102">疑難排解錯誤 404, 找不到檔案</span><span class="sxs-lookup"><span data-stu-id="06e08-102">Troubleshoot Error 404, File not found</span></span>

<span data-ttu-id="06e08-103">當使用者嘗試存取 SharePoint 或 OneDrive 中的網站或檔案時, 會收到錯誤404。</span><span class="sxs-lookup"><span data-stu-id="06e08-103">An Error 404 is received when users are attempting to access a site or file in SharePoint or OneDrive.</span></span> <span data-ttu-id="06e08-104">這通常是因為網站或檔案或群組被重新命名、移動或刪除。</span><span class="sxs-lookup"><span data-stu-id="06e08-104">This is often caused by a site or file or group getting renamed, moved or deleted.</span></span> <span data-ttu-id="06e08-105">例如: 使用者會在嘗試存取根網站集合時遇到404錯誤, 且已被刪除。</span><span class="sxs-lookup"><span data-stu-id="06e08-105">For example: Users will experience a 404 Error attempting to access the Root Site Collection and it has been deleted.</span></span>

<span data-ttu-id="06e08-106">若要解決已重新命名、移動或刪除之網站的錯誤 404:</span><span class="sxs-lookup"><span data-stu-id="06e08-106">To resolve Error 404 for a Site that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="06e08-107">對於位於傳統系統管理中心的傳統網站, 請參閱[還原已刪除的網站集合](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)。</span><span class="sxs-lookup"><span data-stu-id="06e08-107">For classic sites that exist in the Classic Admin Center, see [Restore a deleted site collection](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>


<span data-ttu-id="06e08-108">對於位於新 SharePoint 系統管理中心的新式網站 (通訊、群組連線或其他網站), 請參閱在[新的 sharepoint 系統管理中心中查看及還原刪除的網站](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)。</span><span class="sxs-lookup"><span data-stu-id="06e08-108">For modern sites (communication, group-connected, or other sites) that exist in the new SharePoint admin center, see [View and restore deleted sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection).</span></span>

<span data-ttu-id="06e08-109">若要解決已重新命名、移動或刪除之檔案 (或其他專案) 的錯誤 404:</span><span class="sxs-lookup"><span data-stu-id="06e08-109">To resolve Error 404 for a File (or other item) that has been renamed, moved or deleted:</span></span>

<span data-ttu-id="06e08-110">移至 SharePoint 或 OneDrive 網站, 並從 [網站內容] 中查看 [回收站]。</span><span class="sxs-lookup"><span data-stu-id="06e08-110">Go to the SharePoint or OneDrive site and view the Recycle Bin from the Site contents.</span></span> <span data-ttu-id="06e08-111">請參閱,[還原 SharePoint 網站回收站中的專案](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online)。</span><span class="sxs-lookup"><span data-stu-id="06e08-111">See, [Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/Restore-items-in-the-Recycle-Bin-of-a-SharePoint-site-6df466b6-55f2-4898-8d6e-c0dff851a0be#ID0EAADAAA=Online).</span></span>

<span data-ttu-id="06e08-112">如果您仍無法找到該專案, 您可以在啟用記錄的情況下搜尋 audit 記錄。請參閱[在 Office 365 安全性 & 規範中心內搜尋 audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c)。</span><span class="sxs-lookup"><span data-stu-id="06e08-112">If you are still unable to find the item you can search the audit log if logging is enabled see, [Search the audit log in the Office 365 Security & Compliance Center](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance?redirectSourcePath=%252fclient%252fsearch-the-audit-log-in-the-office-365-security-compliance-center-0d4d0f35-390b-4518-800e-0c7ec95e946c).</span></span>
