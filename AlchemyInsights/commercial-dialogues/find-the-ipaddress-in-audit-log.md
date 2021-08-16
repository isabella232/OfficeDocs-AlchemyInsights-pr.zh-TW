---
title: 在審計記錄檔中尋找 IP 位址
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
ms.openlocfilehash: 5b58803719df700290f495cb2d2d6742f072420a2a1d393534ca165bb5a14fbb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54017123"
---
# <a name="find-the-ip-address-in-audit-log"></a>在審計記錄檔中尋找 IP 位址

1. 對應至使用者或系統管理員所執行之活動的 IP 位址會顯示在審計記錄檔中。 也會記錄用戶端資訊。 以下說明如何識別 IP 位址：

1. 移至[Office 365 安全性 & 規範中心](https://go.microsoft.com/fwlink/p/?linkid=2077143)。
1. 選取 [**搜尋**  >  **[審核記錄搜尋](https://go.microsoft.com/fwlink/?linkid=2103759)**]。
    > [!NOTE]
    > 如果您看到需要開啟審計的通知，請繼續進行，然後立即開啟。 如果未啟用此功能，搜尋結果將無法從先前的日期提取資料。
1. 如果您對特定活動感興趣，請從 [活動] 清單中進行選取，然後按一下 [ **活動** ] 清單。否則，預設會為選取的使用者傳回所有活動。 請注意，[ **活動** ] 功能表中可能無法選取某些活動;不過，如果已選取 [ **顯示所有活動的結果** ] (預設設定) 會傳回這些審計專案。
1. 指定日期範圍，然後在 [ **使用者** ] 欄位中，選取您要調查之使用者的使用者名稱。
1. 選取 **[搜尋]**。 這些活動出現在 **[結果]** 下。 您可以看到每個活動的 IP 位址。
1. 若要查看詳細資料，請選取活動，然後選取 [ **詳細資訊**]。

若要深入瞭解，請參閱搜尋[Office 365 的審計記錄檔，以進行常見案例的疑難排解](https://go.microsoft.com/fwlink/?linkid=2103944)。