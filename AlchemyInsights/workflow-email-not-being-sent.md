---
title: 工作流程電子郵件就不會被傳送
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 261fe1b1bc815dd4ad568051cfefad1e214b957e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530855"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>工作流程電子郵件就不會被傳送 SharePoint 清單或文件庫

1. 從工作流程的電子郵件並不會傳送給所有使用者或只有特定使用者，或您會看到錯誤**電子郵件無法傳送。請確定該電子郵件具有有效收件者**。

    檢查使用者存在於該網站集合的**所有人員**的權限群組 （使用者資訊清單）。  範例直接 URL: https://<tenant>.sharepoint.com/sites/<sitename>/_layouts/15/people.aspx 嗎？MembershipGroupId = 0

    - 如果使用者不存在，請確定使用者登入] 頁面。 
    - 如果是外部使用者，請確定已經接受其邀請。
    - 如果使用者的權限] 群組中存在，請務必電子郵件地址正確無誤。
    - 如果使用者電子郵件地址不在此設定，然後建立該使用者可從的 SharePoint 使用者設定檔會強制使用者帳戶同步處理至這個網站集合的範例警示。
 
2. 從工作流程的電子郵件傳送給網站集合管理員，但未提供給其他使用者，並查看錯誤**HTTP 禁止<span>https:</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.SendEmail**。
 

    請參閱[「 拒絕存取 」 時您電子郵件傳送至 SharePoint 群組](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)。

    此外，確認**限制存取使用者的權限鎖定模式**網站集合功能為非作用中。


## <a name="related-topics"></a>相關主題
想要在 SharePoint Online 中的 Microsoft Flow？
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


