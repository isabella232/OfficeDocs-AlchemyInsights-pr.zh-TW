---
title: 隱藏公用資料夾
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 66c76947d553c32475ebe7a11e69246b5b3a2882bb3d022873d85b93b3e87887
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53945733"
---
# <a name="hide-public-folders"></a>隱藏公用資料夾

**若要隱藏整個公用資料夾樹狀目錄**：

使用[此 ](https://aka.ms/ControlPF) 文章中的步驟，對特定或所有使用者隱藏整個公用資料夾樹狀目錄。

**若要隱藏特定公用資料夾**：

1. 為需要存取公用資料夾的使用者新增權限

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. 從 **[權限]** 清單中移除使用者 **預設**：

    `Remove-PublicFolderClientPermission \test1 -User Default`
