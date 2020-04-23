---
title: 存取拒絕郵件的疑難排解
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759791"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6a735-102">存取拒絕郵件的疑難排解</span><span class="sxs-lookup"><span data-stu-id="6a735-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6a735-103">如果有人收到「拒絕存取」訊息給 SharePoint 中的共用資料夾，則網站集合管理員可能已啟用「限制存取」使用者許可權鎖定模式。」</span><span class="sxs-lookup"><span data-stu-id="6a735-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="6a735-104">若要關閉此功能：</span><span class="sxs-lookup"><span data-stu-id="6a735-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="6a735-105">流覽至網站，按一下 [設定] 圖示，然後按一下 [**網站設定**]。</span><span class="sxs-lookup"><span data-stu-id="6a735-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="6a735-106">按一下 [網站集合管理]\*\*\*\* 下方的 [網站集合功能]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="6a735-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="6a735-107">在 [**限制存取] 使用者許可權鎖定模式**旁，按一下 [**停用**]。</span><span class="sxs-lookup"><span data-stu-id="6a735-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="6a735-108">如果網站是發佈網站，也可以對共用資料夾進行存取被拒絕的訊息。</span><span class="sxs-lookup"><span data-stu-id="6a735-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="6a735-109">如需詳細資訊，請參閱[存取共用資料夾時拒絕存取](https://go.microsoft.com/fwlink/?linkid=2004317)。</span><span class="sxs-lookup"><span data-stu-id="6a735-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="6a735-110">在嘗試查看存取要求時，如果有人收到「拒絕存取」訊息，使用者必須新增為網站集合管理員或網站擁有者群組的成員。</span><span class="sxs-lookup"><span data-stu-id="6a735-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="6a735-111">如需詳細資訊，請參閱拒絕存取「[存取要求」清單](https://go.microsoft.com/fwlink/?linkid=2004220)。</span><span class="sxs-lookup"><span data-stu-id="6a735-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="6a735-112">若使用者從內部部署的 Active Directory 中移除之後收到「拒絕存取」訊息，並將其新增回來，請參閱[在將使用者帳戶同步處理至 Microsoft 365 時，存取權被拒絕](https://go.microsoft.com/fwlink/?linkid=2004318)。</span><span class="sxs-lookup"><span data-stu-id="6a735-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

