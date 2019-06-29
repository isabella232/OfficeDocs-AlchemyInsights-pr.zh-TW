---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/5/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: 5bd6c32a246db9dfcdb475368ade0441df4dc9c3
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365408"
---
# <a name="verify-your-domain"></a><span data-ttu-id="6fdb1-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="6fdb1-102">Verify your domain</span></span>

 <span data-ttu-id="6fdb1-103">**記錄可能尚未在網際網路上更新。**</span><span class="sxs-lookup"><span data-stu-id="6fdb1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="6fdb1-104">通常只需要幾分鐘的時間, 就能看到新的記錄, 但有時可能需要幾個小時的時間。</span><span class="sxs-lookup"><span data-stu-id="6fdb1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="6fdb1-105">如果您已等候長時間, 請仔細檢查您是否已將實際的值複製並貼到您 DNS 主機的 TXT 驗證記錄中。</span><span class="sxs-lookup"><span data-stu-id="6fdb1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="6fdb1-106">常見的問題是記錄中未包含 "MS="。</span><span class="sxs-lookup"><span data-stu-id="6fdb1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="6fdb1-107">我們也需要這個！</span><span class="sxs-lookup"><span data-stu-id="6fdb1-107">We need that too!</span></span>

- <span data-ttu-id="6fdb1-108">在某些 DNS 主機中，您還需要額外採取一個步驟來儲存區域檔案 (DNS 記錄的儲存位置)，以便在網際網路上更新該檔案。</span><span class="sxs-lookup"><span data-stu-id="6fdb1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="6fdb1-109">請確定已儲存您的變更，如此 Office 365 才可以看到並驗證記錄。</span><span class="sxs-lookup"><span data-stu-id="6fdb1-109">Make sure you've saved your changes so Office 365 can see and verify the record.</span></span>
