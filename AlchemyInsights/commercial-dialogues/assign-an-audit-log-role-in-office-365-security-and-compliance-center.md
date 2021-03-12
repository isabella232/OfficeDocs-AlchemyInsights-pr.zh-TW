---
title: 在 Office 365 安全性與合規性中心指派稽核記錄角色
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/21/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7363"
- "9000722"
ms.openlocfilehash: 0eb470b6c17def5517db2f866ef40898b36662ed
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736016"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a>在 Office 365 安全性與合規性中心指派稽核記錄角色

若要搜尋 Office 365 稽核記錄，系統管理員必須在 Exchange Online 中獲派為 **[僅限檢視稽核記錄]** 或 **[稽核記錄]** 角色。 根據預設，這些角色會指派給「合規性管理」和「組織管理」角色群組。 Office 365 和 Microsoft 365 中的全域系統管理員會自動新增為「組織管理」角色群組的成員。

若要讓使用者以最低權限等級搜尋，請在 Exchange Online 中建立自訂角色群組、新增 **僅限檢視稽核記錄** 角色或 **稽核記錄** 角色，然後將使用者新增為新角色群組的成員。

如需詳細資訊，請參閱[管理 Exchange Online 中的角色群組](https://docs.microsoft.com/Exchange/permissions-exo/role-groups)和[在安全性與合規性中心搜尋稽核記錄](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。