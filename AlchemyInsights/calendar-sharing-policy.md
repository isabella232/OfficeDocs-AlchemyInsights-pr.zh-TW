---
title: 618行事曆共用原則
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091585"
---
# <a name="policy-error-when-sharing-a-calendar"></a>共用行事歷時的原則錯誤

1. 請視情況而定，請執行下列其中一項動作：
    - 使用遠端 PowerShell Exchange Online 連線。 如需詳細資訊，請參閱[使用遠端 PowerShell Exchange Online 連線](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)。
    - 在內部部署伺服器上，開啟 [Exchange 管理命令介面]。
2. 決定指派給使用者的共用原則。 若要這麼做，請執行下列命令，並記下傳回的原則：

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. 更新使用者的共用原則。 如果要執行這項操作，請依照下列步驟執行：
    - 開啟 [Exchange 系統管理中心]。
    - 按一下 [ **組織**]，然後按兩下 [ **個人共用**] 下指派給使用者的原則。 這是在步驟2中傳回的原則。
    - 在 [共用規則] 頁面上，在 [ **指定您要共用的資訊**] 下，選取您想要允許的行事曆共用層級。按一下 [ **儲存**]。

如需詳細資訊，請參閱：「 [原則不允許將此層級的許可權授與一個或多個收件者 (s) 」當使用者嘗試共用行事歷時，發生錯誤](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)。
