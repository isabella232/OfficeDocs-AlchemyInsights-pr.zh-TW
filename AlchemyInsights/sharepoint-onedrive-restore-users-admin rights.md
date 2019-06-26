---
title: 對商務用 OneDrive 網站的拒絕存取郵件的疑難排解
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: b394cc1441187133d8829cfc5fb0c1edbd71fd96
ms.sourcegitcommit: 204c8fadd59a597a18ebde24b3c63fbb656ec1b6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/25/2019
ms.locfileid: "35223415"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>對商務用 OneDrive 網站的拒絕存取郵件的疑難排解

當使用者被刪除, 並以相同的使用者主要名稱 (UPN) 重新建立時, 最常發生這個問題。 新帳戶是使用不同的 PUID (Passport 唯一識別碼) 值建立。 當使用者嘗試存取網站集合或其 OneDrive 時, 使用者的 PUID 不正確。 第二個案例包含與 Active Directory 組織單位 (OU) 的目錄同步處理。 如果使用者已經登入 SharePoint, 然後移至不同的 OU, 並透過 SharePoint resynced, 則可能會發生此問題。

若要解決此問題, 您應該使用本文中的步驟, 還原[Office 365 中的使用者](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide), 以還原原始的 UPN。

完成之後, 您可以依照下列步驟來驗證使用者是否具有 OneDrive 網站的系統管理員許可權: 為[使用者的 OneDrive 新增系統管理員](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)

如需許可權等級的詳細資訊, 請參閱[瞭解 SharePoint 中的許可權層級](https://docs.microsoft.com/sharepoint/understanding-permission-levels)一文。
