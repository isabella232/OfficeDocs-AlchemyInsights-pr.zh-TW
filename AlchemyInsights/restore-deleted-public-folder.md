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
ms.openlocfilehash: 7b04612daca61650d162c1dde240e25c1b185b04
ms.sourcegitcommit: 8ba12eff67e405f5922ea4cc35155e3036447859
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2020
ms.locfileid: "42063604"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="083e7-102">還原已刪除的公用資料夾</span><span class="sxs-lookup"><span data-stu-id="083e7-102">Restore a deleted public folder</span></span>

<span data-ttu-id="083e7-103">**若要還原已刪除的公用資料夾中的項目**：</span><span class="sxs-lookup"><span data-stu-id="083e7-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="083e7-104">請參閱[您無法復原刪除的項目從 Outlook 2016 中的非郵件公用資料夾](https://aka.ms/pfrec)。</span><span class="sxs-lookup"><span data-stu-id="083e7-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="083e7-105">**若要還原已刪除的公用資料夾 （的任何類型）**：</span><span class="sxs-lookup"><span data-stu-id="083e7-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="083e7-106">請使用下列 EXO PowerShell 命令：</span><span class="sxs-lookup"><span data-stu-id="083e7-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="083e7-107">語法：</span><span class="sxs-lookup"><span data-stu-id="083e7-107">Syntax:</span></span>

    ><span data-ttu-id="083e7-108">$pf = Get-publicfolder \NON_IPM_SUBTREE\DUMPSTER_ROOT-遞迴 |？{$_.名稱-eq"\<name_of_deleted_public_Folder"};Set-publicfolder $pf.identity-路徑\<還原> 將資料夾的路徑。</span><span class="sxs-lookup"><span data-stu-id="083e7-108">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored></span></span>

    <span data-ttu-id="083e7-109">範例： 下列命令將會還原 Subfolder1，並將它放在 \Parent1 下：</span><span class="sxs-lookup"><span data-stu-id="083e7-109">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    ><span data-ttu-id="083e7-110">$pf = Get-publicfolder \NON_IPM_SUBTREE\DUMPSTER_ROOT-遞迴 |？{$_.名稱-eq"Subfolder1"};Set-publicfolder $pf.identity-路徑 \Parent1</span><span class="sxs-lookup"><span data-stu-id="083e7-110">$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1</span></span>

<span data-ttu-id="083e7-111">如需詳細資訊，請參閱[還原已刪除的公用資料夾](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder)。</span><span class="sxs-lookup"><span data-stu-id="083e7-111">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
