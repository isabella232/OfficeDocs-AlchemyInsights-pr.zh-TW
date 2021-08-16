---
title: 無法存取 SharePoint 或 OneDrive 系統管理中心
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001459"
- "5638"
ms.openlocfilehash: afb28ccae2c9f087f1e1417cb6594cedc908e1cf759a5d1e6d92c4ee9a75527d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020435"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a>無法存取 SharePoint 或 OneDrive 系統管理中心

- 如果您的 SharePoint 或 OneDrive 系統管理中心網站無法存取或無法使用，可能發生暫時的服務問題，即使用者在存取 SharePoint 網站或 OneDrive 內容時遇到間歇性延遲或導覽錯誤。 請查看[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，了解您的組織是否受到影響。

- 您必須將 SharePoint 授權指派給全域和 SharePoint 系統管理員。 剛使用 SharePoint 授權或系統管理員角色指派的新建帳戶，可能會在存取 SharePoint 時遇到問題，例如「拒絕存取」或「找不到使用者」。 請至少等候 24 小時，以完成整個系統的同步處理。 我們知道 24 小時可能感覺有點久。 多數情況下，我們已經著手研究解決方案。

- Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) 如果允許非常短的存取時間，使用者可能會收到拒絕存取，請參閱[拒絕存取 PIM 帳戶](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)。