---
title: 在 Outlook 中新增增益集時，一位使用者收到「拒絕存取」錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: ccb7af8477aba148ddc905448fa5a2b8bd1681443aa67865abfc69e1ca785f75
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076120"
---
# <a name="one-user-gets-access-denied-error-while-adding-add-ins-in-outlook"></a>在 Outlook 中新增增益集時，一位使用者收到「拒絕存取」錯誤

使用者 PowerShell 尋找權限：

Get-ManagementRoleAssignment -RoleAssignee [user@domain.com](mailto:user@domain.com "mailto:user@domain.com") -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType