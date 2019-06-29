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
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380496"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>無法設定主要電子郵件地址或變更使用者屬性

如果您的環境已啟用目錄同步處理, 則無法使用系統管理中心來變更某些使用者或物件屬性。
若要完整管理已同步處理的使用者及其所有屬性, 請使用您的本機 active directory 使用者和群組管理主控台 (adsiedit)。  

或者, 您也可以使用 powershell 變更同步處理使用者的個別使用者或屬性, 如下列常見範例所示: 
- Get-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com"-DisplayName "Test User"-LastName "User"-Title "Manager"-部門 "HR"
- Remove-Get-msoluser-UserPrincipalName "user@yourdomain.onmicrosoft.com