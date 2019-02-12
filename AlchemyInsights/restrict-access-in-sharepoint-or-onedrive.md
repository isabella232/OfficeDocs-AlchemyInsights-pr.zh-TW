---
title: 限制存取 SharePoint 或 OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905139"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="1622a-102">限制存取 SharePoint 或 OneDrive</span><span class="sxs-lookup"><span data-stu-id="1622a-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="1622a-p101">在 SharePoint 和 OneDrive，您限制存取 like 檔案、 資料夾及清單項目僅對群組或個人您想要存取授與存取。根據預設，在 SharePoint 中的權限繼承自較高的最多在階層中。讓檔案會繼承其權限從資料夾、 文件庫，其權限繼承的網站會繼承其權限。</span><span class="sxs-lookup"><span data-stu-id="1622a-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="1622a-p102">您可以共用較高層級 (例如由共用整個網站) 如果您不想要共用網站上的所有項目然後中斷繼承。不過，我們不建議這因為對進行較複雜且費解未來維護的權限。以下是您可以改用：</span><span class="sxs-lookup"><span data-stu-id="1622a-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="1622a-109">如果例如您想要共用但不包括一個檔案的資料夾中的所有內容，請將該檔案移至未共用的新位置。</span><span class="sxs-lookup"><span data-stu-id="1622a-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="1622a-110">如果您有兩個子資料夾中，而且您想要共用一個子資料夾與群組 A 和 B 和允許群組的權限到第二個的子資料夾、 共用與群組的上層資料夾及群組 B 新增到第一個子資料夾。</span><span class="sxs-lookup"><span data-stu-id="1622a-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="1622a-111">停止共用的檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="1622a-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

