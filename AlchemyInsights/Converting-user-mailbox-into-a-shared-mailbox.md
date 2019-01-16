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
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279281"
---
<span data-ttu-id="c789e-p101">您只可以將使用者信箱轉換共用信箱如果使用者具有 Exchange 的授權。信箱轉換後，它會繼續在顯示作用中使用者清單因為該清單包含共用的信箱。不過，已轉換的信箱將也顯示共用的信箱清單中。</span><span class="sxs-lookup"><span data-stu-id="c789e-p101">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license. After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes. However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="c789e-p102">如果您嘗試要轉換的信箱在 Exchange 管理主控台及轉換會失敗，清除您的瀏覽器快取和 cookie，然後再試一次。如果仍然不工作，請嘗試轉換的信箱在 Exchange 管理命令介面中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="c789e-p102">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again. If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="c789e-107">使用中[轉換共用信箱的使用者信箱](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba)的信箱轉換的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="c789e-107">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://support.office.com/client/2e122487-e1f5-4f26-ba41-5689249d93ba).</span></span>
  
