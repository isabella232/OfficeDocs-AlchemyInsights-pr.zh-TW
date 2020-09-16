---
title: 在 Outlook 中新增增益集時，多個使用者收到「拒絕存取」錯誤
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
ms.openlocfilehash: 611a4df473458abc0ab0c65442f2141763f7b868
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47724354"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a>在 Outlook 中新增增益集時，多個使用者收到「拒絕存取」錯誤

您可以指定組織中的哪些系統管理員具有安裝及管理 Outlook 增益集的權限。 您也可以指定組織中的哪些使用者有權限安裝及管理供其本身使用的增益集。

如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins)。

若要確認您已成功指派使用者的權限，請以要驗證的角色名稱取代 <Role Name>，然後在 Exchange Online PowerShell 中執行下列命令：

Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers

此範例說明如何驗證您已指派給哪些人從組織的 Office 市集安裝增益集的權限。

PowerShell

-Role "Org Marketplace Apps" -GetEffectiveUsers

在 Get-ManagementRoleAssignment 的結果中，檢閱 [有效使用者] 欄中的項目。

如需詳細的語法和參數資訊，請參閱 [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment)。
 