---
title: 未傳送工作流程電子郵件
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1586"
ms.openlocfilehash: 7efb8895ac7e2816a2c6055ec3c08d6f7029d39d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748980"
---
# <a name="workflow-email-is-not-being-sent-for-a-sharepoint-list-or-library"></a>未傳送 SharePoint 清單或文件庫的工作流程電子郵件

1. 來自工作流程的電子郵件不會傳送給所有使用者或只傳送給特定使用者，否則您會看到錯誤 **電子郵件無法傳送。請確定電子郵件具有有效的收件**者。

    檢查使用者是否存在於該網站集合的 [ **所有人員** ] 許可權群組中 (使用者資訊清單) 。  URL: <tenant> sharepoint.com/sites/ <sitename> /_layouts/15/people.aspx 的範例 direct？MembershipGroupId = 0

    - 如果使用者不存在，請確定使用者已登入頁面。 
    - 如果是外部使用者，請確定已接受其邀請。
    - 如果使用者確實存在於許可權群組中，請確定電子郵件地址正確無誤。
    - 若未在這裡設定使用者的電子郵件地址，則會為該使用者建立範例警示，以強制將該使用者帳戶從 SharePoint 的使用者設定檔同步處理至此網站集合。
 
2. 來自工作流程的電子郵件會傳送給網站集合管理員，但不會傳送給其他使用者，也不會查看錯誤 **HTTP 禁止訪問 <span>HTTPs：</span>//URL/_vti_bin/client.xvc.sp.utilities.utility.sendemail**。
 

    [當您傳送電子郵件給 SharePoint 群組時，](https://docs.microsoft.com/sharepoint/support/sharing-and-permissions/access-denied-when-send-an-email-to-groups)請參閱「拒絕存取」。

    此外，請確認「 **限制存取使用者許可權鎖定模式** 」網站集合功能未作用中。


## <a name="related-topics"></a>相關主題
想要在 SharePoint Online 中試用 Microsoft 流程嗎？
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


