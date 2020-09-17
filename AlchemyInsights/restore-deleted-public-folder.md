---
title: 還原已刪除的公用資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774522"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="f0544-102">還原已刪除的公用資料夾</span><span class="sxs-lookup"><span data-stu-id="f0544-102">Restore a deleted public folder</span></span>

<span data-ttu-id="f0544-103">**若要從公用資料夾還原已刪除的專案**：</span><span class="sxs-lookup"><span data-stu-id="f0544-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="f0544-104">請參閱 [您無法從 Outlook 2016 中的非郵件公用資料夾復原已刪除的郵件](https://aka.ms/pfrec)。</span><span class="sxs-lookup"><span data-stu-id="f0544-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="f0544-105">\*\*若要還原已刪除的公用資料夾 (任何類型) \*\*：</span><span class="sxs-lookup"><span data-stu-id="f0544-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="f0544-106">請使用下列 EXO PowerShell 命令：</span><span class="sxs-lookup"><span data-stu-id="f0544-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="f0544-107">語法：</span><span class="sxs-lookup"><span data-stu-id="f0544-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="f0544-108">範例：下列命令會還原 Subfolder1，並將其置於 \Parent1 中：</span><span class="sxs-lookup"><span data-stu-id="f0544-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="f0544-109">如需詳細資訊，請參閱 [還原已刪除的公用資料夾](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 。</span><span class="sxs-lookup"><span data-stu-id="f0544-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
