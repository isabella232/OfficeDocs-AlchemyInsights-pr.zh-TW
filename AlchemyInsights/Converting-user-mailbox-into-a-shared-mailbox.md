---
title: 將使用者信箱轉換成共用信箱吗？
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: reference
ms.service: o365-administration
localization_priority: Priority
ROBOTS: NOINDEX, NOFOLLOW
description: ''
ms.openlocfilehash: 22ad1b3fb818b40bcd77974031735f931e986968
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460390"
---
您只可以將使用者信箱轉換共用信箱如果使用者具有 Exchange 的授權。信箱轉換後，它會繼續在顯示作用中使用者清單因為該清單包含共用的信箱。不過，已轉換的信箱將也顯示共用的信箱清單中。 
  
如果您嘗試要轉換的信箱在 Exchange 管理主控台及轉換會失敗，清除您的瀏覽器快取和 cookie，然後再試一次。如果仍然不工作，請嘗試轉換的信箱在 Exchange 管理命令介面中執行下列命令：
  
```
Set-Mailbox -Type Shared
```

使用中[轉換共用信箱的使用者信箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)的信箱轉換的詳細資訊。
  
