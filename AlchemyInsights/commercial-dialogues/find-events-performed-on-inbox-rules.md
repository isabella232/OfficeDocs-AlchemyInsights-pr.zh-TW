---
title: 尋找對收件匣規則執行的事件
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: deb83d278a2b398b4ea6fc31b043c33309b736e3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50464502"
---
# <a name="find-events-performed-on-inbox-rules"></a>尋找對收件匣規則執行的事件

建立、變更或刪除收件匣規則時，事件會記錄在審計記錄檔中。 以下說明如何進行檢查：

1. 移至 [Office 365 的安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 選取 [搜尋] > [審計記錄搜尋]。

    > [!NOTE]
    > 如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 若未開啟此功能，搜尋結果將無法從先前的日期提取資料。
1. 選取 [活動] 欄位，並尋找 Exchange 信箱活動，然後選取 [New-InboxRule 從 Outlook Web App 建立收件匣規則]。 當您完成時，按一下窗格外以最小化 [活動] 窗格。
1. 指定日期範圍，然後在 [使用者] 欄位中，選取您要調查之使用者的使用者名稱。 您可以一次選取一個以上的使用者。
1. 選取 [搜尋]。 活動會顯示在 [結果] 底下。
1. 若要查看詳細資料，請選取活動，然後選取 [詳細資訊]。 在 [參數] 區段中，您可以看到規則的名稱、條件集，以及規則將採取的動作。

若要深入瞭解，請參閱搜尋 Office 365 audit log 以進行常見案例疑難排解。