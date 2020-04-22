---
title: Verify your domain
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
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
ms.openlocfilehash: 2c4d8e075d2cf7214b5ef005b856daf7fb0ed53c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710434"
---
# <a name="verify-your-domain"></a><span data-ttu-id="c340a-102">Verify your domain</span><span class="sxs-lookup"><span data-stu-id="c340a-102">Verify your domain</span></span>

 <span data-ttu-id="c340a-103">**該記錄可能尚未在網際網路上更新。**</span><span class="sxs-lookup"><span data-stu-id="c340a-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="c340a-104">這通常只需要幾分鐘的時間，我們才能看到新的記錄，但是有時候它可能需要數小時的時間。</span><span class="sxs-lookup"><span data-stu-id="c340a-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="c340a-105">如果您已等候長時間，請加倍檢查您是否已將確切的值複製並貼到 DNS 主機上的 TXT 驗證記錄中。</span><span class="sxs-lookup"><span data-stu-id="c340a-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="c340a-106">常見的問題是記錄中未包含 "MS="。</span><span class="sxs-lookup"><span data-stu-id="c340a-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="c340a-107">我們也需要這個！</span><span class="sxs-lookup"><span data-stu-id="c340a-107">We need that too!</span></span>

- <span data-ttu-id="c340a-108">在某些 DNS 主機中，您還需要額外採取一個步驟來儲存區域檔案 (DNS 記錄的儲存位置)，以便在網際網路上更新該檔案。</span><span class="sxs-lookup"><span data-stu-id="c340a-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="c340a-109">請確認您已儲存您的變更，讓 Microsoft 可以查看和驗證記錄。</span><span class="sxs-lookup"><span data-stu-id="c340a-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
