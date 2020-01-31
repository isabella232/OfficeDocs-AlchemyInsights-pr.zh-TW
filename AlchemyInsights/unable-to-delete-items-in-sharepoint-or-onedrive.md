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
ms.openlocfilehash: abfcb91c6040aeed759d697ca63546ccea8ede97
ms.sourcegitcommit: c5e800313a6f211386a384716e5fa18e7fcc8c1c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/28/2020
ms.locfileid: "41571229"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="f36a5-102">無法刪除項目</span><span class="sxs-lookup"><span data-stu-id="f36a5-102">Unable to delete items</span></span>

<span data-ttu-id="f36a5-103">保留原則可能會導致此，您必須停用或排除此問題所造成的個別保留。</span><span class="sxs-lookup"><span data-stu-id="f36a5-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="f36a5-104">會移除保留原則或保留之後，可能需要 24 小時的時間，變更才會生效。</span><span class="sxs-lookup"><span data-stu-id="f36a5-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="f36a5-105">請確定沒有在[保留原則](https://docs.microsoft.com/office365/securitycompliance/retention-policies)設定的項目。</span><span class="sxs-lookup"><span data-stu-id="f36a5-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="f36a5-106">網站可能已超過儲存限制、 增加的[網站配額](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)和刪除的項目。</span><span class="sxs-lookup"><span data-stu-id="f36a5-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="f36a5-107">確保項目不是另一個使用者[取出](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de)。</span><span class="sxs-lookup"><span data-stu-id="f36a5-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="f36a5-108">最後，系統管理員可以使用[SharePoint 典範與實例](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation)(PnP) 其中包含文件庫的 PowerShell 命令，可讓您在執行複雜的管理動作，例如強制刪除頑固項目。</span><span class="sxs-lookup"><span data-stu-id="f36a5-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="f36a5-109">移除 PNP 檔案</span><span class="sxs-lookup"><span data-stu-id="f36a5-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="f36a5-110">移除 PNP 資料夾</span><span class="sxs-lookup"><span data-stu-id="f36a5-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="f36a5-111">移除 PNP 清單項目</span><span class="sxs-lookup"><span data-stu-id="f36a5-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="f36a5-112">移除 PNP 清單</span><span class="sxs-lookup"><span data-stu-id="f36a5-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="f36a5-113">移除 PNP 欄位 （欄）</span><span class="sxs-lookup"><span data-stu-id="f36a5-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)