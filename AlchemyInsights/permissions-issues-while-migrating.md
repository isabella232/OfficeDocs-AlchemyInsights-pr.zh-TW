---
title: 遷移時的許可權問題
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: cbec51a7-5513-4848-a9ae-cdf993e000a8
ms.openlocfilehash: 077b7cf29ef6a40ef7f2aebef15e39a0f5df0fc3
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758961"
---
# <a name="user-profile-and-photo-synchronization"></a><span data-ttu-id="05d7c-102">使用者設定檔和相片同步處理</span><span class="sxs-lookup"><span data-stu-id="05d7c-102">User Profile and Photo synchronization</span></span>

 <span data-ttu-id="05d7c-103">**設定檔相片同步**處理-使用者可能會注意到，使用者的設定檔照片並未同步處理至 SharePoint。</span><span class="sxs-lookup"><span data-stu-id="05d7c-103">**Profile Photo Synchronization** - Users may notice that their profile photo is not synchronizing to SharePoint.</span></span> <span data-ttu-id="05d7c-104">或者，他們可能嘗試更新其設定檔相片，而且該相片仍會顯示舊的相片。</span><span class="sxs-lookup"><span data-stu-id="05d7c-104">Or, they may have tried to update their profile photo and the photo still appears as the old photo.</span></span> <span data-ttu-id="05d7c-105">若要確定設定檔相片如預期所示，使用者將需要啟動照片同步處理。</span><span class="sxs-lookup"><span data-stu-id="05d7c-105">To ensure the profile photo shows as expected, the user will need to initiate a photo sync.</span></span> 
  
<span data-ttu-id="05d7c-106">如需有關相片同步處理常式的詳細資訊，請參閱[Microsoft 365 中有關設定檔圖片同步處理的資訊](https://go.microsoft.com/fwlink/?linkid=2022634)。</span><span class="sxs-lookup"><span data-stu-id="05d7c-106">For more information about the photo synchronization process, see [Information about profile picture synchronization in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2022634)</span></span>
  
- <span data-ttu-id="05d7c-107">**設定檔同步**處理-完成設定檔同步處理所需的時間取決於 AD 匯入工作必須處理的變更數目（[工時]）。</span><span class="sxs-lookup"><span data-stu-id="05d7c-107">**Profile Synchronization** - The time that's required to complete a profile synchronization depends on the number of changes (work) the AD Import Job has to process.</span></span> <span data-ttu-id="05d7c-108">如果有許多變更，計時器工作有許多工作要執行，而且會花更長的時間來反映使用者設定檔應用程式中的變更。</span><span class="sxs-lookup"><span data-stu-id="05d7c-108">If there are many changes, the timer job has a lot of work to do, and it will take longer for the changes to be reflected in the User Profile Application.</span></span> <span data-ttu-id="05d7c-109">如果計時器工作有少量的工作要執行，則變更會在使用者設定檔應用程式中更快速地反映出來。</span><span class="sxs-lookup"><span data-stu-id="05d7c-109">If the timer job has a small volume of work to do, the changes will be reflected in the User Profile Application much faster.</span></span> 
  
<span data-ttu-id="05d7c-110">如需有關設定檔同步處理常式的詳細資訊，請參閱[SharePoint Online 中使用者設定檔同步處理的相關資訊](https://go.microsoft.com/fwlink/?linkid=2022639)。</span><span class="sxs-lookup"><span data-stu-id="05d7c-110">For more information about the profile synchronization process, see [Information about user profile synchronization in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2022639)</span></span>
    
- <span data-ttu-id="05d7c-111">**Update Profile In Office delve** -delve 使用者可以管理其 Microsoft 365 設定檔。</span><span class="sxs-lookup"><span data-stu-id="05d7c-111">**Update Profile in Office Delve** - Delve users can manage their Microsoft 365 Profile.</span></span> <span data-ttu-id="05d7c-112">如需詳細資訊，請參閱[在 Office Delve 中查看和更新您的設定檔](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba)。</span><span class="sxs-lookup"><span data-stu-id="05d7c-112">For more information, see [View and Update your profile in Office Delve](https://support.office.com/article/View-and-update-your-profile-in-Office-Delve-4e84343b-eedf-45a1-aeb9-8627ccca14ba).</span></span>
    

