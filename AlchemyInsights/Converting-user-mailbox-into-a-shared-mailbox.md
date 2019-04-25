---
title: 將使用者信箱轉換成共用信箱？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 4da54121763fd33aa111f3bb3c26963cd271dc51
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32374314"
---
您就只能將使用者信箱轉換為共用信箱如果使用者擁有的 Exchange 授權。 轉換信箱後，它會繼續顯示在作用中使用者清單中因為該清單包含共用的信箱。 不過，轉換的信箱會也顯示在共用的信箱清單中。 
  
如果您嘗試轉換 Exchange 系統管理主控台中的信箱，但轉換失敗，清除您的瀏覽器快取和 cookie，然後再試一次。 如果仍無法正常，請嘗試轉換的信箱在 Exchange 管理命令介面中執行下列命令：
  
```
Set-Mailbox -Type Shared
```

使用中[轉換為共用信箱的使用者信箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)的信箱轉換的詳細資訊。
  
