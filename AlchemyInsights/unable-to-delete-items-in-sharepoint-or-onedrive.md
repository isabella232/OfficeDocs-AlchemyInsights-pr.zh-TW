---
title: 無法刪除 SharePoint 或 OneDrive 中的項目
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: cc19fcb6603160032dac52b1ec9e194a90b7891f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049508"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="b8815-102">無法刪除項目</span><span class="sxs-lookup"><span data-stu-id="b8815-102">Unable to delete items</span></span>

<span data-ttu-id="b8815-103">有問題刪除 SharePoint 項目嗎？</span><span class="sxs-lookup"><span data-stu-id="b8815-103">Having issues deleting SharePoint items?</span></span>

- <span data-ttu-id="b8815-104">永遠確定您已刪除的項目或已移除之項目的[網站集合管理員](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)嘗試[適當的權限](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)。</span><span class="sxs-lookup"><span data-stu-id="b8815-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="b8815-105">請確定沒有在[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定的項目。</span><span class="sxs-lookup"><span data-stu-id="b8815-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="b8815-106">確保項目不是另一個使用者[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)。</span><span class="sxs-lookup"><span data-stu-id="b8815-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="b8815-107">最後，系統管理員可以使用[SharePoint 典範與實例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) 其中包含文件庫的 PowerShell 命令，可讓您在執行複雜的管理動作，例如強制刪除頑固項目。</span><span class="sxs-lookup"><span data-stu-id="b8815-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="b8815-108">移除 PNP 檔案</span><span class="sxs-lookup"><span data-stu-id="b8815-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="b8815-109">移除 PNP 資料夾</span><span class="sxs-lookup"><span data-stu-id="b8815-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="b8815-110">移除 PNP 清單項目</span><span class="sxs-lookup"><span data-stu-id="b8815-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="b8815-111">移除 PNP 清單</span><span class="sxs-lookup"><span data-stu-id="b8815-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="b8815-112">移除 PNP 欄位 （欄）</span><span class="sxs-lookup"><span data-stu-id="b8815-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)