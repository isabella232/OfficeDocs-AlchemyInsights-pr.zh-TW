---
title: 管理同步處理的使用者
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823958"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>無法設定主要電子郵件地址、變更使用者屬性或移除/刪除同步處理的使用者

如果為您的環境啟用目錄同步處理，則無法使用 Microsoft 365 系統管理中心變更部分使用者或物件屬性。

若要完全管理同步處理的使用者及其所有屬性，請使用您的本機 active directory 使用者和群組管理主控台 (adsi) 。  

或者，您也可以使用 powershell 變更個別使用者或屬性，以進行同步處理的使用者，如下列常見範例所示：

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
