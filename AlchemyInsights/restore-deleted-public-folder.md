---
title: 還原已刪除的公用資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158484"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="f8f38-102">還原已刪除的公用資料夾</span><span class="sxs-lookup"><span data-stu-id="f8f38-102">Restore a deleted public folder</span></span>

<span data-ttu-id="f8f38-103">**若要還原已刪除的公用資料夾中的項目**：</span><span class="sxs-lookup"><span data-stu-id="f8f38-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="f8f38-104">請參閱[您無法復原刪除的項目從 Outlook 2016 中的非郵件公用資料夾](https://aka.ms/pfrec)。</span><span class="sxs-lookup"><span data-stu-id="f8f38-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="f8f38-105">**若要還原已刪除的公用資料夾 （的任何類型）**：</span><span class="sxs-lookup"><span data-stu-id="f8f38-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="f8f38-106">請使用下列 EXO PowerShell 命令：</span><span class="sxs-lookup"><span data-stu-id="f8f38-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="f8f38-107">語法：</span><span class="sxs-lookup"><span data-stu-id="f8f38-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="f8f38-108">範例： 下列命令將會還原 Subfolder1，並將它放在 \Parent1 下：</span><span class="sxs-lookup"><span data-stu-id="f8f38-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="f8f38-109">如需詳細資訊，請參閱[還原已刪除的公用資料夾](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)。</span><span class="sxs-lookup"><span data-stu-id="f8f38-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
