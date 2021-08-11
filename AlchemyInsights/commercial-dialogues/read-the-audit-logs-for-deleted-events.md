---
title: 讀取已刪除事件的審計記錄檔
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
ms.openlocfilehash: 8d656d5660b7c6e6d32d32a06c3dbf49c45e4ca04c4422128f1c4ea62413afa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53967324"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>讀取已刪除事件的審計記錄檔

以下說明如何執行此動作：

1. 移至[Office 365 安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 選取 [**搜尋**  >  [**審核記錄搜尋**](https://go.microsoft.com/fwlink/?linkid=2103759)]。
    > [!NOTE]
    > 如果您看到需要開啟此功能的通知，請繼續進行並開啟它。 如果未開啟此功能，搜尋結果將無法從先前的日期提取資料。
1. 選取 [**活動**]，然後尋找 **Exchange 信箱活動**。 選取 [刪除的郵件] 資料夾 **中已刪除的郵件** ，並將 **郵件移至 [刪除** 的郵件] 資料夾選項。 當您完成時，按一下窗格外以最小化 [ **活動** ] 窗格。
1. 指定日期範圍，然後在 [ **使用者** ] 方塊中，選取您要調查之使用者的使用者名稱。 您可以一次選取一個以上的使用者。
1. 選取 **[搜尋]**。 這些活動出現在 **[結果]** 下。
1. 若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。 在 [ **AffectedItems** ] 欄位中會顯示刪除專案的其他資訊，例如專案的主旨行和位置。
    > [!NOTE]
    > 您無法使用「審核記錄」功能還原已刪除的專案。 若要還原刪除的專案，請參閱[復原已刪除的郵件或 Outlook Web App 中的電子郵件](https://go.microsoft.com/fwlink/?linkid=2103759)。

若要深入瞭解，請參閱[搜尋 Office 365 的審計記錄檔，以進行常見案例的疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。
