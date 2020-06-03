---
title: 無法刪除 SharePoint 或 OneDrive 中的專案
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
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511967"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="7cf06-102">無法刪除專案</span><span class="sxs-lookup"><span data-stu-id="7cf06-102">Unable to delete items</span></span>

<span data-ttu-id="7cf06-103">保留原則可能會造成這種情況，您必須停用或排除導致此問題的個別保留。</span><span class="sxs-lookup"><span data-stu-id="7cf06-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="7cf06-104">在刪除保留原則或保留後，最多可能需要24小時的時間，變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="7cf06-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="7cf06-105">確定沒有專案的[保留原則](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)設定。</span><span class="sxs-lookup"><span data-stu-id="7cf06-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="7cf06-106">網站可能已超過儲存量限制、增加[網站配額](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)，以及刪除專案。</span><span class="sxs-lookup"><span data-stu-id="7cf06-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="7cf06-107">確定專案尚未[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)給另一位使用者。</span><span class="sxs-lookup"><span data-stu-id="7cf06-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="7cf06-108">最後，系統管理員可以使用[SharePoint 的模式和慣例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)（PnP），其中包含 PowerShell 命令的文件庫，可讓您執行複雜的管理動作，例如強制刪除 stubborn 專案。</span><span class="sxs-lookup"><span data-stu-id="7cf06-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="7cf06-109">移除 PNP 檔</span><span class="sxs-lookup"><span data-stu-id="7cf06-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="7cf06-110">移除 PNP 資料夾</span><span class="sxs-lookup"><span data-stu-id="7cf06-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="7cf06-111">移除 PNP 清單專案</span><span class="sxs-lookup"><span data-stu-id="7cf06-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="7cf06-112">移除 PNP 清單</span><span class="sxs-lookup"><span data-stu-id="7cf06-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="7cf06-113">移除 PNP 欄位（欄）</span><span class="sxs-lookup"><span data-stu-id="7cf06-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)