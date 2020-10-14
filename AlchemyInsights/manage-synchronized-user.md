---
title: 管理同步處理的使用者
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
- "9000609"
- "2444"
ms.openlocfilehash: 7bf7d3f00308ff6bc973cd52e09ca51c5fd0f45b
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/13/2020
ms.locfileid: "48451391"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>無法設定主要電子郵件地址、變更使用者屬性或移除/刪除同步處理的使用者

如果為您的環境啟用目錄同步處理，則無法使用 Microsoft 365 系統管理中心變更部分使用者或物件屬性。

若要完全管理同步處理的使用者及其所有屬性，請使用您的本機 active directory 使用者和群組管理主控台 (adsi) 。  

或者，您也可以使用 powershell 變更個別使用者或屬性，以進行同步處理的使用者，如下列常見範例所示：

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
