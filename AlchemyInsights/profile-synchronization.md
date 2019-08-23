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
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554324"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a><span data-ttu-id="be7c5-102">何時執行動作我的設定檔變更同步處理至 SharePoint 使用者設定檔應用程式？</span><span class="sxs-lookup"><span data-stu-id="be7c5-102">When do my profile changes sync to the SharePoint User Profile Application?</span></span>

<span data-ttu-id="be7c5-103">SharePoint Online 會使用 Active Directory 匯入計時器服務 （AD 匯入） 匯入至使用者設定檔應用程式的使用者和群組。</span><span class="sxs-lookup"><span data-stu-id="be7c5-103">SharePoint Online uses the Active Directory Import timer job (AD Import) to import users and groups into the User Profile Application.</span></span> 
  
1. <span data-ttu-id="be7c5-104">AD 匯入同步使用者設定檔應用程式從 SharePoint Online 目錄存放區的變更。</span><span class="sxs-lookup"><span data-stu-id="be7c5-104">AD Import syncs changes from the SharePoint Online Directory Store to the User Profile Application.</span></span> <span data-ttu-id="be7c5-105">這些變更會分批處理。</span><span class="sxs-lookup"><span data-stu-id="be7c5-105">These changes are processed in batches.</span></span>
    
2. <span data-ttu-id="be7c5-106">計時器工作執行之前所做的變更會同步處理。</span><span class="sxs-lookup"><span data-stu-id="be7c5-106">The timer job runs until the changes are synced.</span></span>
    
> [!NOTE]
> <span data-ttu-id="be7c5-107">要執行的工作所花費的時間取決於變更處理程序數目。</span><span class="sxs-lookup"><span data-stu-id="be7c5-107">The time it takes the job to run depends on the number of changes to process.</span></span> <span data-ttu-id="be7c5-108">大量變更耗時越久。</span><span class="sxs-lookup"><span data-stu-id="be7c5-108">A large number of changes takes longer.</span></span> <span data-ttu-id="be7c5-109">服務層級協議 (SLA) 會指出使用者在 SharePoint Online 目錄中的變更會反映使用者設定檔應用程式中，在 24 小時內。</span><span class="sxs-lookup"><span data-stu-id="be7c5-109">The Service Level Agreement (SLA) states that a change to a user in the SharePoint Online Directory will be reflected in the User Profile Application in 24 hours.</span></span> 
  
[<span data-ttu-id="be7c5-110">在 SharePoint Online 中的使用者設定檔同步處理的詳細資訊</span><span class="sxs-lookup"><span data-stu-id="be7c5-110">More info about user profile sync in SharePoint Online</span></span>](https://go.microsoft.com/fwlink/?linkid=875671)
  

