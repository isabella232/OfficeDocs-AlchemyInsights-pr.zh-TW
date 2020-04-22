---
title: 存取拒絕郵件的疑難排解
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 82e11458529b8a49e583b1a6963a51e2a466bfd6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758372"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>在 Sharepoint/OneDrive 系統管理中心中存取拒絕郵件的疑難排解

如果您在嘗試流覽 Sharepoint/OneDrive 系統管理中心時收到「拒絕存取」訊息，請確定您已[將授權指派給使用者](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。 如果使用者有授權，您也應確定已將其[指派給系統管理員角色](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)，可存取系統管理中心。

當使用者使用相同的使用者主體名稱（UPN）加以刪除及重新建立時，也會發生此問題。 新帳戶是使用不同的 PUID （Passport 唯一識別碼）值建立。 當使用者嘗試存取網站集合或其 OneDrive 時，使用者的 PUID 不正確。 第二個案例是與 Active Directory 組織單位（OU）進行目錄同步處理。 如果使用者已經登入 SharePoint，然後將其移至不同的 OU，並使用 SharePoint 進行 resynced，可能會發生此問題。

若要解決此問題，您應該使用本文中的步驟還原原始的 UPN，在[Microsoft 365 中還原使用者](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)。

附注：如果您的 OneDrive 或 SharePoint 系統管理中心無法供之前有存取權的多個使用者使用，則可能會發生暫時的服務問題。  [檢查服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。


