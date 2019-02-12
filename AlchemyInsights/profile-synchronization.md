---
title: 設定檔同步處理
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: d1a72a85767e36fefbfa8eee266befcaf2e48af0
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29920079"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="77854-102">何時 「 我的設定檔變更同步處理至 SharePoint 使用者設定檔應用程式？</span><span class="sxs-lookup"><span data-stu-id="77854-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="77854-103">SharePoint Online 使用 Active Directory 匯入計時器服務 （AD 匯入） 的使用者和群組匯入使用者設定檔應用程式。</span><span class="sxs-lookup"><span data-stu-id="77854-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="77854-p101">AD 匯入同步 SharePoint Online 目錄存放區之使用者設定檔應用程式的變更。這些變更會分批處理。</span><span class="sxs-lookup"><span data-stu-id="77854-p101">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application. These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="77854-106">計時器工作執行之前所做的變更會同步處理。</span><span class="sxs-lookup"><span data-stu-id="77854-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="77854-p102">若要執行之工作所花費的時間取決於處理修訂的數目。變更大量花費的時間。服務層級協議 (SLA) 會指出使用者的 SharePoint Online 目錄中的變更反映使用者設定檔應用程式中時在 24 小時。</span><span class="sxs-lookup"><span data-stu-id="77854-p102">The time it takes the job to run depends on the number of changes to process. A large number of changes takes longer. The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="77854-110">在 SharePoint Online 中的使用者設定檔同步處理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="77854-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

