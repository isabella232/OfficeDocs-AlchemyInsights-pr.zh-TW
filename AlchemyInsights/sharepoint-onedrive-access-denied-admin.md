---
title: 針對 「 拒絕存取 」 訊息進行疑難排解
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760332"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>疑難排解 Sharepoint/OneDrive 系統管理中心中的 「 拒絕存取 」 訊息

如果您會收到拒絕存取訊息嘗試瀏覽至 Sharepoint/OneDrive 系統管理中心時，請確定該您[指派授權給使用者](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。 如果使用者擁有授權，您也應該要確定他們已[指派給系統管理員角色](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide)可以存取系統管理中心。

當使用者是刪除並重新建立具有相同使用者主體名稱 (UPN)，也會發生這個問題。 使用不同的 PUID （Passport 唯一識別碼） 值，會建立新的帳戶。 當使用者嘗試存取網站集合或其 OneDrive 時，使用者會有不正確的 PUID。 第二個案例牽涉到目錄同步處理與 Active Directory 組織單位 (OU)。 如果使用者有已登入至 SharePoint]，然後會移至不同的 OU 和 resynced 與 SharePoint，否則可能會發生這個問題。

若要解決此問題，您應還原原始的 UPN 與在文章中，[將還原的使用者在 Office 365 中](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)的步驟。

附註： 如果無法使用先前持有存取的多個使用者的 OneDrive 或 SharePoint 系統管理員中心，有可能是暫時的服務問題。  [檢查服務健康狀況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。


