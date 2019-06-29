---
title: 在審核記錄檔中識別 IP 位址和用戶端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382944"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>在審核記錄檔中識別 IP 位址和用戶端

對應至使用者或系統管理員活動的 IP 位址會顯示在 [Audit 記錄檔] 中。 也會記錄用戶端資訊。 以下是識別此類資訊的步驟

1. 登入[Office 365 安全性 & 規範中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。

   如果您對特定活動感興趣, 請從 [**活動**] 清單中選取。 如果不是, 則會傳回所選使用者的所有活動 (預設設定)。

   **附注**: 某些活動可能無法在 [**活動**] 功能表中使用;不過, 如果選取 [**顯示所有活動的結果**] (預設設定), 則會傳回這些審計專案。

3. 在 [使用者] 欄位中指定**使用者**名稱, 為活動選取適當的日期範圍, 然後按一下 [**搜尋**]。

在結果中, 您可以在 [結果] 窗格中看到該活動的 IP 位址。 選取 [審核記錄], 以查看**詳細資料**快顯視窗中的詳細資訊 (例如, 用戶端、執行動作的使用者等等)。

如需詳細資訊, 請參閱[尋找用來存取已遭破壞之帳戶之電腦的 IP 位址](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。
