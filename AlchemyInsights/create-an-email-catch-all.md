---
title: 建立電子郵件全部
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286060"
---
# <a name="create-an-email-catch-all"></a>建立電子郵件全部

使用的全部是強烈建議不要。 最好是提供退回回給您，讓寄件者知道為解決讓他們可以採取的動作無法傳遞郵件寄件者。 您也可以限制為僅限以前有效的電子郵件地址受監視的信箱。 

任何全部信箱將會收到了很多垃圾郵件，並可能最終填滿，如果不密切監視。 （還有接收限制）。 

如果您決定要繼續，請遵循下列步驟：

1. 建立動態通訊群組 & 包含 「 所有收件者類型 >。

2. 建立專用的信箱來捕捉電子郵件，例如 catchall@domain.com。

3. 為特定網域，設定 「 InternalRelay 」 至 DomainType。 如果您稍後移除全部，請務必設定為 [授權網域。

4. 建立郵件流程傳輸規則，如下所示：

    - 如果寄件者為 「 外部組織 」
    - 將郵件重新導向至 Catchall@domain.com
    - 除非收件者屬於的 allusers@domain.com （通訊群組包含所有成員）
    - 確保以驗證新的信箱會新增至動態通訊群組
