---
title: 建立電子郵件全部捕獲
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712977"
---
# <a name="create-an-email-catch-all"></a>建立電子郵件全部捕獲

強烈建議使用全部捕獲。 更好的方式是提供回復寄件者，讓寄件者知道其郵件無法依照處理方式傳遞，這樣他們才可以採取動作。 您也可以將受監控的信箱限制為只捕捉先前有效的電子郵件地址。 

任何捕獲所有的信箱都會收到大量的垃圾郵件，而且可能會最終填滿（如果未密切監視）。  (有接收限制。 )  

如果您決定繼續，請執行下列步驟：

1. 建立動態通訊群組 & 包括「所有收件者類型」。

2. 建立專用的信箱以捕捉電子郵件，例如，catchall@domain.com。

3. 針對特定網域，將 DomainType 設定為 "InternalRelay"。 如果您稍後移除 [全部捕捉]，請務必將網域設回 [授權]。

4. 建立郵件流程傳輸規則，如下所示：

    - 如果寄件者是「組織外」
    - 將郵件重新導向至 Catchall@domain.com
    - 除非收件者是 allusers@domain.com 的成員，否則 (通訊群組中包含所有成員) 
    - 確定已將新的信箱新增至動態通訊群組
