---
title: 設定檔同步處理
ms.author: arnek
author: arnek
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: dc6e0280961d14aa3e6bd466afbe0cbe89418d17
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768104"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="c3445-102">我的設定檔變更何時同步處理至 SharePoint 的使用者設定檔應用程式？</span><span class="sxs-lookup"><span data-stu-id="c3445-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="c3445-103">SharePoint 線上使用 Active Directory 匯入計時器工作（AD 匯入）將使用者和群組匯入使用者設定檔應用程式。</span><span class="sxs-lookup"><span data-stu-id="c3445-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="c3445-104">AD 匯入將 SharePoint 線上目錄存放區中的變更同步處理至使用者設定檔應用程式。</span><span class="sxs-lookup"><span data-stu-id="c3445-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="c3445-105">這些變更會以批次處理。</span><span class="sxs-lookup"><span data-stu-id="c3445-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="c3445-106">計時器工作會在同步處理變更之前執行。</span><span class="sxs-lookup"><span data-stu-id="c3445-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="c3445-107">執行工作所需的時間取決於要處理的變更數目。</span><span class="sxs-lookup"><span data-stu-id="c3445-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="c3445-108">大量的變更所需的時間較長。</span><span class="sxs-lookup"><span data-stu-id="c3445-108">A large number of changes takes longer.</span></span> <span data-ttu-id="c3445-109">服務等級協定（SLA）規定在使用者設定檔應用程式中，會在24小時內反映 SharePoint 線上目錄中使用者的變更。</span><span class="sxs-lookup"><span data-stu-id="c3445-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="c3445-110">SharePoint Online 中使用者設定檔同步處理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="c3445-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

