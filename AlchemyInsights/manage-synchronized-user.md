---
title: 管理同步處理的使用者
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407341"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>無法設定主要電子郵件地址、變更使用者屬性或移除/刪除同步處理的使用者

如果為您的環境啟用目錄同步處理，則無法使用 Microsoft 365 系統管理中心變更部分使用者或物件屬性。

若要完全管理同步處理的使用者及其所有屬性，請使用您的本機 active directory 使用者和群組管理主控台（adsi .msc）。  

或者，您也可以使用 powershell 變更個別使用者或屬性，以進行同步處理的使用者，如下列常見範例所示： 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
