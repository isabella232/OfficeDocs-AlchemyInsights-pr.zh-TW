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
ms.openlocfilehash: ab34b8939b95b29bedb797f640dd744bc783adef
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36496390"
---
# <a name="convert-a-user-mail-box-into-a-shared-mailbox"></a><span data-ttu-id="8deb4-102">將使用者的郵件] 方塊中選取轉換成共用信箱</span><span class="sxs-lookup"><span data-stu-id="8deb4-102">Convert a user mail box into a shared mailbox</span></span>

<span data-ttu-id="8deb4-103">您就只能將使用者信箱轉換為共用信箱如果使用者擁有的 Exchange 授權。</span><span class="sxs-lookup"><span data-stu-id="8deb4-103">You can only convert a user mailbox to a shared mailbox if the user has an Exchange license.</span></span> <span data-ttu-id="8deb4-104">轉換信箱後，它會繼續顯示在作用中使用者清單中因為該清單包含共用的信箱。</span><span class="sxs-lookup"><span data-stu-id="8deb4-104">After the mailbox is converted, it will continue to show up in the active users list because that list includes shared mailboxes.</span></span> <span data-ttu-id="8deb4-105">不過，轉換的信箱會也顯示在共用的信箱清單中。</span><span class="sxs-lookup"><span data-stu-id="8deb4-105">However, the converted mailbox will also show up in the shared mailbox list.</span></span> 
  
<span data-ttu-id="8deb4-106">如果您嘗試轉換 Exchange 系統管理主控台中的信箱，但轉換失敗，清除您的瀏覽器快取和 cookie，然後再試一次。</span><span class="sxs-lookup"><span data-stu-id="8deb4-106">If you try to convert a mailbox in the Exchange Admin Console and the conversion fails, clear your browser cache and cookies and try again.</span></span> <span data-ttu-id="8deb4-107">如果仍無法正常，請嘗試轉換的信箱在 Exchange 管理命令介面中執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="8deb4-107">If it still isn't working, try converting the mailbox in the Exchange Management Shell by running the following command:</span></span>
  
```
Set-Mailbox -Type Shared
```

<span data-ttu-id="8deb4-108">使用中[轉換為共用信箱的使用者信箱](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox)的信箱轉換的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="8deb4-108">More mailbox conversion information is available in [Convert a user mailbox to a shared mailbox](https://docs.microsoft.com/office365/admin/email/convert-user-mailbox-to-shared-mailbox).</span></span>
  
