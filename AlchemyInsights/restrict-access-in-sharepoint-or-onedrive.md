---
title: 限制存取 SharePoint 或 OneDrive 中
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551442"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="30c68-102">限制存取 SharePoint 或 OneDrive 中</span><span class="sxs-lookup"><span data-stu-id="30c68-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="30c68-103">在 SharePoint 和 OneDrive，您限制存取等檔案、 資料夾及清單項目僅對群組或個人您希望擁有權限授與存取。</span><span class="sxs-lookup"><span data-stu-id="30c68-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="30c68-104">根據預設，在 SharePoint 中的權限被繼承自階層中的較高向上。</span><span class="sxs-lookup"><span data-stu-id="30c68-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="30c68-105">因此檔案是繼承其權限的資料夾，文件庫，是它的權限繼承的網站是繼承其權限。</span><span class="sxs-lookup"><span data-stu-id="30c68-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="30c68-106">您可以在較高層級共用 (例如所共用的整個網站) 如果您不想要共用網站上的所有項目，然後中斷繼承。</span><span class="sxs-lookup"><span data-stu-id="30c68-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="30c68-107">不過，我們不建議這因為它使得較複雜且令人費解日後維護的權限。</span><span class="sxs-lookup"><span data-stu-id="30c68-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="30c68-108">以下是您可以改為:</span><span class="sxs-lookup"><span data-stu-id="30c68-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="30c68-109">如果您要共用資料夾，但不包括一個檔案中的所有內容，例如，將該檔案移至新的位置不共用。</span><span class="sxs-lookup"><span data-stu-id="30c68-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="30c68-110">如果您有兩個的子資料夾在資料夾中，而且您想要與 A 和 B 的群組共用一個子資料夾及只允許群組的存取第二個的子資料夾、 父項資料夾共用與群組的第一個子資料夾中加入群組 B。</span><span class="sxs-lookup"><span data-stu-id="30c68-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="30c68-111">停止共用檔案或資料夾</span><span class="sxs-lookup"><span data-stu-id="30c68-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

