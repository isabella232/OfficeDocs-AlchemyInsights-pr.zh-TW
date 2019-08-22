---
title: 管理已同步處理的使用者
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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541973"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>無法設定主要電子郵件地址或變更使用者屬性

如果您的環境啟用目錄同步處理，則無法使用 Microsoft 365 系統管理中心變更部分使用者或物件的屬性。

若要完全管理同步處理的使用者和其所有屬性，使用本機 active directory 使用者和群組管理主控台 (adsiedit.msc)。  

或者，您可以變更個別使用者或使用 powershell 例如這些常見的範例所示的同步處理使用者的屬性： 
- Set-msoluser-UserPrincipalName user@yourdomain.onmicrosoft.com-AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Set-msoluser-UserPrincipalName"user@yourdomain.onmicrosoft.com"-DisplayName"Test User"-LastName"User"-標題 「 管理員 」 的 「 人力資源 」 部門
- Remove-msoluser UserPrincipalName 」 user@yourdomain.onmicrosoft.com