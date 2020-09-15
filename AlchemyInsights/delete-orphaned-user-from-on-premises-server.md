---
title: 從內部部署的伺服器刪除孤立使用者
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/20/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1725"
- "9000179"
ms.openlocfilehash: 537ae7edebfa5a4ab71c2141d549d732ed4f883f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680126"
---
# <a name="delete-orphaned-user-from-on-premises-server"></a>從內部部署的伺服器刪除孤立使用者

若要移除孤立使用者，請依循下列步驟：

1. 按照[什麼是 Azure Active Directory 的混合式身分識別？](https://technet.microsoft.com/library/jj151771.aspx#bkmk_synchronizedirectories) (英文) 中的指示，強制執行目錄同步處理。

2. 若要驗證目錄同步處理，請參閱[什麼是 Azure Active Directory 的混合式身分識別？](https://technet.microsoft.com/library/jj151797.aspx) (英文)。

3. 如果同步處理功能正常，但是 Active Directory 物件刪除並未傳播到 Azure AD，請使用下列其中一種適用於 Windows PowerShell Cmdlet 的 Azure Active Directory 模組來手動移除孤立物件：

    Remove-MsolContact  
    Remove-MsolGroup  
    Remove-MsolUser

    例如，若要移除原本使用目錄同步處理所建立的孤立使用者識別碼 john.smith@contoso.com，請執行 Cmdlet：

    Remove-MsolUser –UserPrincipalName John.Smith@Contoso.com