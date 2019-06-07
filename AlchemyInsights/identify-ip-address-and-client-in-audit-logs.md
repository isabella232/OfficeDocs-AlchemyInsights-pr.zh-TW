---
title: 識別 IP 位址和稽核記錄中的用戶端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 87e0d414fe02d5074a56cd5a77d50db1464b7faf
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752051"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>識別 IP 位址和稽核記錄中的用戶端

會對應至使用者或系統管理員活動的 IP 位址會顯示在稽核記錄檔。 用戶端資訊也會記錄。 以下是用於識別此類資訊的步驟

1. 登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)

2. 按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。

   如果您有興趣的特定活動，請從**活動**清單中選取。 如果沒有，所選的使用者 （預設值） 會傳回所有活動。

   **附註**： 某些活動可能無法在 [**活動**] 功能表中;不過，這些稽核項目將會傳回**所有活動顯示結果**是否已選取 （預設值）。

3. 在 [**使用者**] 欄位中指定的使用者名稱，選取適當的日期範圍的活動，，然後按一下 [**搜尋**。

在結果中，您可以看到該活動在結果窗格中的 IP 位址。 選取 [稽核記錄，以查看**詳細資料**彈出式視窗 （例如，用戶端，執行巨集指令、 等等的使用者。） 中的詳細的資訊。

如需詳細資訊，請參閱[尋找用來存取遭入侵的帳戶之電腦的 IP 位址](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。
