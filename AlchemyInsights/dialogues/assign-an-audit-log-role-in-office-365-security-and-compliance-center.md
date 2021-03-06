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
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50509653"
---
# <a name="assign-an-audit-log-role-in-the-office-365-security--compliance-center"></a><span data-ttu-id="c2d66-102">在 Office 365 安全性與合規性中心指派稽核記錄角色</span><span class="sxs-lookup"><span data-stu-id="c2d66-102">Assign an Audit Log role in the Office 365 Security & Compliance Center</span></span>

<span data-ttu-id="c2d66-103">若要搜尋 Office 365 稽核記錄，系統管理員必須在 Exchange Online 中獲派為 **[僅限檢視稽核記錄]** 或 **[稽核記錄]** 角色。</span><span class="sxs-lookup"><span data-stu-id="c2d66-103">To search the Office 365 audit log, an administrator must be assigned the **View-Only Audit Logs** role or the **Audit Logs** role in Exchange Online.</span></span> <span data-ttu-id="c2d66-104">根據預設，這些角色會指派給「合規性管理」和「組織管理」角色群組。</span><span class="sxs-lookup"><span data-stu-id="c2d66-104">These roles are assigned to the Compliance Management and Organization Management role groups by default.</span></span> <span data-ttu-id="c2d66-105">Office 365 和 Microsoft 365 中的全域系統管理員會自動新增為「組織管理」角色群組的成員。</span><span class="sxs-lookup"><span data-stu-id="c2d66-105">Global administrators in Office 365 and Microsoft 365 are automatically added as members of the Organization Management role group.</span></span>

<span data-ttu-id="c2d66-106">若要讓使用者以最低權限等級搜尋，請在 Exchange Online 中建立自訂角色群組、新增 **僅限檢視稽核記錄** 角色或 **稽核記錄** 角色，然後將使用者新增為新角色群組的成員。</span><span class="sxs-lookup"><span data-stu-id="c2d66-106">To enable a user to search with the minimum level of privileges, create a custom role group in Exchange Online, add the **View-Only Audit Logs** role or **Audit Logs** role, and then add the user as a member of the new role group.</span></span>

<span data-ttu-id="c2d66-107">如需詳細資訊，請參閱[管理 Exchange Online 中的角色群組](https://docs.microsoft.com/Exchange/permissions-exo/role-groups)和[在安全性與合規性中心搜尋稽核記錄](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)。</span><span class="sxs-lookup"><span data-stu-id="c2d66-107">For more information, see [Manage role groups in Exchange Online](https://docs.microsoft.com/Exchange/permissions-exo/role-groups) and [Search the audit log in the Security & Compliance Center](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance).</span></span>