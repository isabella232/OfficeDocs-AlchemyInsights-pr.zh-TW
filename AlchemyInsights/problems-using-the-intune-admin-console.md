---
title: 使用 Intune 系統管理員主控台時發生問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "46523017"
---
# <a name="problems-using-the-intune-admin-console"></a>使用 Intune 系統管理員主控台時發生問題

**瀏覽 Intune 系統管理入口網站時「拒絕存取」。**

- 如果您是 Intune 自訂角色的成員，請確認您的帳戶已獲指派 Intune 或 Enterprise Mobility Suite (EMS) 授權。
- 如果您使用 Configuration Manager 管理裝置，請確認您不屬於 Configuration Manager MDM 的 Intune 使用者集合。
- 請確認您在 Intune 角色刀鋒視窗中已獲指派適當的角色型系統管理控制 (RBAC) 權限。
- 請確認使用的群組不是通訊群組清單。 Azure 入口網站中的 Intune 僅支援屬於 Azure Active Directory 安全性群組的使用者帳戶。 請檢閱 Azure 入口網站中的群組 > **[Intune]** > **[群組]**，或 Azure 入口網站 > **[Azure Active Directory]**。

**使用者對於獲指派的 Intune 角色擁有太多權限**

建議使用者移至 **[Intune]** > **[Intune 角色]** > **[我的權限]** > **[匯出]**，以檢閱獲授與的權限。

**我已將範圍群組新增至角色，但該角色的使用者仍然看得到其他使用者或裝置。**

範圍群組不會篩選出使用者或裝置。 範圍群組：

- 限制使用者能夠指派原則或應用程式的對象。
- 只允許特定使用者在裝置上執行遠端工作。

如需有關範圍群組的詳細資訊，請參閱[使用 Microsoft Intune 的角色型存取控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。

**我已經將使用者新增至 Intune 角色，但他們仍然擁有 Intune 系統管理員主控台的完整存取權。**

瀏覽至 Intune > Azure 入口網站中的 **[使用者]**，並確認使用者未獲指派 Azure 入口網站中的下列任何角色：

- 全域系統管理員
- Intune 服務系統管理員
- SharePoint 系統管理員

如需詳細資訊，請參閱[使用 Microsoft Intune 的角色型存取控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。

**Access 問題**

如需詳細資訊，請參閱[無法登入 Office 365、Azure 或 Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)。