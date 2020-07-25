---
title: 在 Outlook 中新增增益集時，一位使用者收到「拒絕存取」錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 1f4672e306a282b3e1d20c75f4e361c02cdddaed
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/24/2020
ms.locfileid: "45397702"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>在 Outlook 中新增增益集時，一位使用者收到「拒絕存取」錯誤

使用者 PowerShell 尋找權限：

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType