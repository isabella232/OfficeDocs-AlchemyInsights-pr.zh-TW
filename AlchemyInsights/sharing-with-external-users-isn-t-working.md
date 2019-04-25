---
title: 與外部使用者共用無法正常運作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 69e290e5a13f40ad045086791189a7d0af88240b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32369489"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="1d5d1-102">修正問題與外部使用者共用 SharePoint 內容</span><span class="sxs-lookup"><span data-stu-id="1d5d1-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="1d5d1-103">請確定您的組織外部共用開啟：</span><span class="sxs-lookup"><span data-stu-id="1d5d1-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="1d5d1-104">移至[服務&amp;增益集] 頁面上，在 Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，並按一下 [**網站**]。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="1d5d1-105">請確定設定已開啟 [「 開啟 」。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="1d5d1-106">如果已選取 「 唯一現有外部使用者 」，請確認外部使用者會列在 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="1d5d1-107">請確定網站開啟外部共用它。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="1d5d1-108">傳統網站集合：</span><span class="sxs-lookup"><span data-stu-id="1d5d1-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="1d5d1-109">在 [新 SharePoint 系統管理中心中，在左邊窗格中，按一下 [**網站**]。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="1d5d1-110">選取的網站或網站，以及功能區上，按一下 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="1d5d1-111">小組網站屬於 Office 365 群組，或是通訊網站：</span><span class="sxs-lookup"><span data-stu-id="1d5d1-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="1d5d1-112">這些新的網站類型有相同共用設定為您整個組織的設定，除非整個組織的設定可讓共用檔案使用不需要登入的連結。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="1d5d1-113">在此情況下，網站會允許與新的和現有的外部使用者登入共用。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="1d5d1-114">若要變更特定網站的設定，請使用新的 SharePoint 系統管理中心或 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="1d5d1-115">[解更多](https://go.microsoft.com/fwlink/?linkid=871863)。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="1d5d1-116">可以比您整個組織的設定，但不是更寬鬆比全組織的設定更嚴格的站台中的外部共用設定。</span><span class="sxs-lookup"><span data-stu-id="1d5d1-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

