---
title: 在 SharePoint 或 OneDrive 中限制存取權
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715875"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="1f857-102">在 SharePoint 或 OneDrive 中限制存取權</span><span class="sxs-lookup"><span data-stu-id="1f857-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="1f857-103">在 SharePoint 和 OneDrive 中，您可以只將存取權授與您想要存取的群組或個人，來限制存取檔、資料夾和清單等專案。</span><span class="sxs-lookup"><span data-stu-id="1f857-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="1f857-104">根據預設，SharePoint 中的許可權會從階層中較高的位置繼承。</span><span class="sxs-lookup"><span data-stu-id="1f857-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="1f857-105">因此，檔案會從該資料夾繼承其許可權，該資料夾會從該資料夾繼承其許可權，而這些許可權會從該網站繼承許可權。</span><span class="sxs-lookup"><span data-stu-id="1f857-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="1f857-106">您可以在較高的層次（如共用整個網站）進行共用，如果您不想共用網站上的所有專案，則中斷繼承。</span><span class="sxs-lookup"><span data-stu-id="1f857-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="1f857-107">不過，我們不建議您這麼做，因為它會使許可權在未來變得更複雜且令人困惑。</span><span class="sxs-lookup"><span data-stu-id="1f857-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="1f857-108">以下是您可以執行的動作：</span><span class="sxs-lookup"><span data-stu-id="1f857-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="1f857-109">例如，如果您想要共用資料夾中除了一個檔案之外的所有內容，請將該檔案移至未共用的新位置。</span><span class="sxs-lookup"><span data-stu-id="1f857-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="1f857-110">如果資料夾中有兩個子資料夾，而且想要與群組 A 和 B 共用一個子資料夾，而且只允許群組存取第二個子資料夾，請與群組 A 共用父項資料夾，並將 B 群組新增至第一個子資料夾。</span><span class="sxs-lookup"><span data-stu-id="1f857-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="1f857-111">停止共用檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="1f857-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

