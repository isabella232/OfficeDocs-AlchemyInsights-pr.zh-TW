---
title: 在審核記錄中識別 IP 位址和用戶端
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 080b3df3934781ebf0d0cd5243787bf6975fc5f123b5b1593c0b6d9ada4eae5d
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887491"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>在審核記錄中識別 IP 位址和用戶端

Microsoft 365 使用者或系統管理員所對應之活動的 IP 位址會顯示在審核記錄檔中。 也會記錄用戶端資訊。 以下是識別這類資訊的步驟

1. 登入[Microsoft 365 規範中心](https://protection.office.com/)。

2. 移至 [**搜尋**  >  **審核記錄搜尋**] 頁面。

   如果您對特定的活動感興趣，請從 [ **活動** ] 清單中進行選取。 如果不是，則會針對選取的使用者 (預設設定) 傳回所有活動。

   **附注**： [ **活動** ] 功能表中可能無法使用某些活動;不過，如果已選取 [ **顯示所有活動的結果** ] (預設設定) 會傳回這些審計專案。

3. 在 [使用者] 欄位中指定 **使用者** 名稱，針對活動選取適當的日期範圍，然後按一下 [ **搜尋**]。

在結果中，您可以在 [結果] 窗格中查看該活動的 IP 位址。 選取 [ **詳細資料** ] 快顯視窗中的詳細資訊 (例如，用戶端、執行動作的使用者等等 ) 。

如需詳細資訊，請參閱 [尋找用來存取已遭破壞之帳戶之電腦的 IP 位址](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。
