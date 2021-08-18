---
title: 在審計記錄檔中識別刪除郵件事件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7e13c9e5fbfa6ade065c2810150687085c1a9daae1a11c134688ec9a83ad37d9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54115639"
---
# <a name="audit-logs-for-deleted-email-messages"></a>已刪除電子郵件的審計記錄

從2019年1月開始，Microsoft 預設會開啟信箱審核記錄。 否則，若要查看特定使用者的刪除郵件事件，您必須手動啟用審核的刪除動作。 如果已為您的組織或特定使用者啟用信箱審核記錄，請遵循下列步驟。

1. 登入[Microsoft 365 規範中心](https://protection.office.com/)

2. 按一下 [ **搜尋和調查** ]，然後選取 [ **審核記錄搜尋**]。

3. 在 [ **開始日期** ] 和 [ **結束日期** ] 欄位中，選取日期範圍。 指定您要調查之使用者的使用者名稱)  (刪除專案的使用者。 在 [**活動**] 欄位中，選取 [**刪除的郵件] 資料夾中已刪除的郵件**，並 **將郵件移至 [刪除的郵件**

4. 按一下 [搜尋]。

在結果中，選取一個審計記錄。 在 [詳細資料] 快顯視窗中，按一下 [ **詳細資訊**]。 已刪除專案的其他資訊 (例如，刪除專案的主旨行和位置) 會顯示在 [ **AffectedItems** ] 欄位中。 **ClientInfoString** 屬性會顯示是否 Outlook 中發生刪除，Outlook 網頁版 (先前稱為 Outlook Web App) 或任何其他裝置。

如需詳細資訊，請參閱 [決定誰設定信箱的電子郵件](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)轉寄功能。

**附注**：您無法使用「審核記錄」功能來取得刪除的專案。 若要在 Outlook 網頁版中取得已刪除的郵件，請參閱[在 Outlook Web App 中復原已刪除的](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)郵件。
