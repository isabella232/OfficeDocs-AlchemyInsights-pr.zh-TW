---
title: 無法刪除 SharePoint 或 OneDrive 中的專案
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366524"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="10456-102">無法刪除專案</span><span class="sxs-lookup"><span data-stu-id="10456-102">Unable to delete items</span></span>

<span data-ttu-id="10456-103">在刪除專案時有問題嗎？</span><span class="sxs-lookup"><span data-stu-id="10456-103">Having issues deleting items?</span></span>

- <span data-ttu-id="10456-104">請務必確定您有[適當的許可權](https://docs.microsoft.com/sharepoint/default-sharepoint-groups)可刪除專案, 或讓[網站集合管理員](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator)嘗試移除專案。</span><span class="sxs-lookup"><span data-stu-id="10456-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="10456-105">確定專案上沒有[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定。</span><span class="sxs-lookup"><span data-stu-id="10456-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="10456-106">確定專案未[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)給另一位使用者。</span><span class="sxs-lookup"><span data-stu-id="10456-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="10456-107">最後, 系統管理員可以使用[SharePoint 模式和作法](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP), 其中包含 PowerShell 命令庫, 可讓您執行複雜的管理動作, 例如強制刪除 stubborn 的專案。</span><span class="sxs-lookup"><span data-stu-id="10456-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="10456-108">移除 PNP 檔案</span><span class="sxs-lookup"><span data-stu-id="10456-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="10456-109">移除 PNP 資料夾</span><span class="sxs-lookup"><span data-stu-id="10456-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="10456-110">移除 PNP 清單專案</span><span class="sxs-lookup"><span data-stu-id="10456-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="10456-111">移除 PNP 清單</span><span class="sxs-lookup"><span data-stu-id="10456-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="10456-112">移除 PNP 欄位 (資料行)</span><span class="sxs-lookup"><span data-stu-id="10456-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)