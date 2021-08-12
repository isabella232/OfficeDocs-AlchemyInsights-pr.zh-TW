---
title: 還原已刪除的公用資料夾
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943366"
---
# <a name="restore-a-deleted-public-folder"></a>還原已刪除的公用資料夾

**若要從公用資料夾還原已刪除的專案**：

- 請參閱[您無法從 Outlook 2016 中的非郵件公用資料夾復原已刪除的郵件](https://aka.ms/pfrec)。
 
**若要還原已刪除的公用資料夾 (任何類型)**： 

- 請使用下列 EXO PowerShell 命令：

    語法：

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    範例：下列命令會還原 Subfolder1，並將其置於 \Parent1 中：

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

如需詳細資訊，請參閱 [還原已刪除的公用資料夾](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) 。
