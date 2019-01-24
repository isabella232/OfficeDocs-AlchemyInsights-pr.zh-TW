---
title: 疑難排解 「 拒絕存取 」 訊息
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460109"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="57abf-102">疑難排解 「 拒絕存取 」 訊息</span><span class="sxs-lookup"><span data-stu-id="57abf-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="57abf-p101">如果某人收到的 「 拒絕存取 」 訊息至共用資料夾，為網站集合管理員可能會有已啟用 「 限制存取使用者權限鎖定模式 」 中。若要關閉這：</span><span class="sxs-lookup"><span data-stu-id="57abf-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="57abf-105">瀏覽至網站、 按一下 [設定] 圖示，並再按一下 [**網站設定**]。</span><span class="sxs-lookup"><span data-stu-id="57abf-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="57abf-106">在 [網站集合管理] 下，按一下 [網站集合功能]。</span><span class="sxs-lookup"><span data-stu-id="57abf-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="57abf-107">**限制存取使用者權限鎖定模式**] 旁的 [**停用**。</span><span class="sxs-lookup"><span data-stu-id="57abf-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="57abf-p102">如果站台是發佈網站的 「 拒絕存取 」 訊息可以也會發生的共用資料夾。資訊，請參閱[「 拒絕存取 」 時存取共用的資料夾](https://go.microsoft.com/fwlink/?linkid=2004317)。</span><span class="sxs-lookup"><span data-stu-id="57abf-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="57abf-p103">如果某人 got 「 拒絕存取 」 訊息嘗試檢視存取權要求時，使用者必須新增為網站集合管理員或網站擁有人群組的成員。如需詳細資訊，請參閱[「 拒絕存取 」 存取權要求清單](https://go.microsoft.com/fwlink/?linkid=2004220)。</span><span class="sxs-lookup"><span data-stu-id="57abf-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="57abf-112">如果使用者收到的 「 拒絕存取 」 訊息之後他們已從 Active Directory 內部部署中移除，然後加後，請參閱[「 拒絕存取 」 時的使用者帳戶同步處理至 Office 365](https://go.microsoft.com/fwlink/?linkid=2004318)。</span><span class="sxs-lookup"><span data-stu-id="57abf-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

