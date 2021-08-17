---
title: 單一使用者在 Outlook 中沒有看見增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 647a17bb5220d3591934c4f53cf417d42810b2c1a681bafd3e2d703abbfcbc64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050649"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a>單一使用者在 Outlook 中沒有看見增益集

使用者可能屬於不具備正確 AppsForOfficeEnabled 參數的角色。 請執行此 Cmdlet，找出正確的角色是否與使用者相關聯：

Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType

如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。
