---
title: 全域和 SharePoint 系統管理員
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
- "9002962"
- "5674"
ms.openlocfilehash: 03a76d22f1370234442afe455b4b898a37dd796b7d795c7ab1190ddd3102ae11
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056409"
---
# <a name="global-and-sharepoint-admin"></a>全域和 SharePoint 系統管理員

您必須將 SharePoint 授權指派給全域和 SharePoint 系統管理員。 剛使用 SharePoint 授權或系統管理員角色指派的新建帳戶，可能會在存取 SharePoint 時遇到問題，例如「拒絕存取」或「找不到使用者」。 請至少等候 24 小時，以完成整個系統的同步處理。 我們知道 24 小時可能感覺有點久。 多數情況下，我們已經著手研究解決方案。

獲派全域或 SharePoint 系統管理員角色的使用者可以存取 SharePoint 系統管理中心，還可以建立及管理網站 (之前稱為「網站集合」)、指定網站系統管理員、管理共用設定等。 他們無法自動存取所有網站和每個使用者的 OneDrive，但他們可以授與自己權限，來存取存取任何網站或 OneDrive。 他們也可以使用 Microsoft PowerShell 來管理 SharePoint 和 OneDrive。

若要深入了解，請參閱[關於 Microsoft 365 中的 SharePoint 系統管理員角色](https://docs.microsoft.com/sharepoint/sharepoint-admin-role)。
Microsoft SharePoint 或 Microsoft OneDrive 變成無法存取的原因可能有數個。 如果您無法存取 SharePoint Online，請使用下列指南來解決此問題。

- [無法存取 SharePoint Online](https://docs.microsoft.com/sharepoint/troubleshoot/sharing-and-permissions/sharepoint-online-inaccessible)

- [SharePoint 或 OneDrive 系統管理中心中受 PIM 管理的使用者帳戶遭到拒絕存取](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)