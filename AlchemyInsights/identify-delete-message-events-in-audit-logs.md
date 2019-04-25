---
title: 識別刪除稽核記錄中的郵件事件
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416701"
---
# <a name="audit-logs-for-deleted-email-messages"></a>稽核記錄檔的已刪除的電子郵件訊息

2019 年 1 月開始，信箱稽核記錄預設會開啟 Microsoft。 否則，若要檢閱刪除特定使用者的郵件事件，您需要以手動啟用稽核的刪除動作。 如果信箱稽核記錄已啟用您的組織或特定使用者，請遵循下列步驟。

1. 登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。

3. 在 [**開始日期**和**結束日期**] 欄位中選取日期範圍。 指定您想要調查 （使用者刪除的項目） 的使用者的使用者名稱。 在 [**活動**] 欄位中，選取 [**刪除的項目資料夾中的已刪除郵件**和**Moved 郵件提交至刪除的項目] 資料夾**。

4. Click **Search**.

在結果中，選取 [稽核記錄]。 在詳細資料彈出式視窗中，按一下 [**更多的資訊**。 已刪除的項目 （例如，[主旨] 行和時已刪除之項目的位置） 的其他資訊會顯示在 [ **AffectedItems** ] 欄位。 **ClientInfoString**屬性將會顯示在 Outlook 中，Outlook （先前稱為 Outlook Web App） 或任何其他裝置上是否發生刪除。

如需詳細資訊，請參閱 <<c0>的判斷設定電子郵件轉寄的信箱。

**附註**： 您無法擷取已刪除的項目使用的稽核記錄功能。 若要擷取網頁型 Outlook 中已刪除的郵件，請參閱[復原已刪除的 Outlook Web App 中的項目](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)。
