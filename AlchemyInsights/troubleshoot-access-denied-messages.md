---
title: 針對 「 拒絕存取 」 訊息進行疑難排解
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: e4fea7188bd77ba876e2a245414372c3ff836059
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36500387"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="44c8f-102">針對 「 拒絕存取 」 訊息進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="44c8f-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="44c8f-103">如果某人會收到 「 拒絕存取 」 訊息到 SharePoint 中的共用資料夾，網站集合管理員，可能就已啟用 「 限制存取使用者的權限鎖定模式。 」</span><span class="sxs-lookup"><span data-stu-id="44c8f-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="44c8f-104">若要關閉此功能：</span><span class="sxs-lookup"><span data-stu-id="44c8f-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="44c8f-105">瀏覽至網站，按一下 [設定] 圖示，然後按一下 [**網站設定]**。</span><span class="sxs-lookup"><span data-stu-id="44c8f-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="44c8f-106">按一下 [網站集合管理]\*\*\*\* 下方的 [網站集合功能]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="44c8f-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="44c8f-107">**限制存取使用者的權限鎖定模式**] 旁按一下 [**停用**]。</span><span class="sxs-lookup"><span data-stu-id="44c8f-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="44c8f-108">如果網站是發佈網站的 「 拒絕存取 」 訊息可以也會發生的共用資料夾。</span><span class="sxs-lookup"><span data-stu-id="44c8f-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="44c8f-109">如需資訊，請參閱[存取的共用的資料夾時，拒絕存取](https://go.microsoft.com/fwlink/?linkid=2004317)。</span><span class="sxs-lookup"><span data-stu-id="44c8f-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="44c8f-110">如果嘗試檢視存取權要求時，有人會收到 「 拒絕存取 」 訊息，使用者必須新增為網站集合管理員或網站擁有者群組的成員。</span><span class="sxs-lookup"><span data-stu-id="44c8f-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="44c8f-111">如需詳細資訊，請參閱[「 拒絕存取 」 存取權要求清單](https://go.microsoft.com/fwlink/?linkid=2004220)。</span><span class="sxs-lookup"><span data-stu-id="44c8f-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="44c8f-112">如果他們已移除 Active Directory-從內部，並再新增回後，使用者會收到 「 拒絕存取 」 訊息，請參閱[「 拒絕存取 」 時的使用者帳戶同步處理到 Office 365](https://go.microsoft.com/fwlink/?linkid=2004318)。</span><span class="sxs-lookup"><span data-stu-id="44c8f-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

