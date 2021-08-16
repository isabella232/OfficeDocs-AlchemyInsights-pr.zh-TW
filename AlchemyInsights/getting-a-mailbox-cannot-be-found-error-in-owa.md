---
title: 126在 OWA 中找不到信箱錯誤？
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: aca0371dad9ba43fa21b0df8e50f1b8ee536528af90d6bda401995c6e5796be4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54056481"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>是否收到在 Outlook 網頁版中找不到信箱的錯誤？

如果您使用 Outlook 網頁版，但找不到 **信箱的** 錯誤，則您用來連線到 Outlook 網頁版的帳戶沒有 Exchange Online 授權，因此沒有信箱與帳戶相關聯。 您的系統管理員可以指派授權至您的帳戶，依照下列步驟進行：

1. 開啟 [ [Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/homepage)]，然後移至 [**使用者**] 區段下的 [作用中的 **使用者**]，然後選取看到錯誤的使用者。

2. 在開啟的使用者頁面中，移至 [**授權與應用程式**] 區段中，選取適當的 **位置** 值，並指派包含 Exchange Online (的授權，以查看其詳細資料) 。 完成後，按一下 [儲存變更 **]**。

在某些情況下，如果授權已指派給使用者帳戶，移除並重新指派授權可協助解決問題，並在系統中正確布建： 

- 檢查您的 M365 Exchange Online (和其他，如果您有任何) 訂閱是最新的，且最近未到期。

確定您的訂閱尚未到期，且已將有效的授權指派給使用者帳戶後，就可能需要24小時的時間才能進行授權的布建，所以您可能需要等待您的問題解決。 如需詳細資訊，請參閱 [指派及管理授權](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)。