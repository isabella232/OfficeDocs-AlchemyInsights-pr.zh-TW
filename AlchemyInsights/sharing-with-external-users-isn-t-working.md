---
title: 與外部使用者共用無法運作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 37da77c73b3abbdcf9cb2b9c4c43f31eea3c0a49
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912993"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="d9478-102">修正與外部使用者 SharePoint 內容共用的問題</span><span class="sxs-lookup"><span data-stu-id="d9478-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="d9478-103">請確定您的組織已開啟外部共用：</span><span class="sxs-lookup"><span data-stu-id="d9478-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="d9478-104">移至[Microsoft 365 &amp;系統管理中心中的 [服務增益集] 頁面](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，然後按一下 [**網站**]。</span><span class="sxs-lookup"><span data-stu-id="d9478-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="d9478-105">確定設定已開啟「開啟」。</span><span class="sxs-lookup"><span data-stu-id="d9478-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="d9478-106">如果選取 [只是現有的外部使用者]，請確定外部使用者已列在 Microsoft 365 系統管理中心中。</span><span class="sxs-lookup"><span data-stu-id="d9478-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="d9478-107">請確定網站已開啟外部共用。</span><span class="sxs-lookup"><span data-stu-id="d9478-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="d9478-108">針對傳統網站集合：</span><span class="sxs-lookup"><span data-stu-id="d9478-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="d9478-109">在 [新增 SharePoint 系統管理中心] 的左窗格中，按一下 [**網站**]。</span><span class="sxs-lookup"><span data-stu-id="d9478-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="d9478-110">選取網站，然後按一下功能區上的 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="d9478-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="d9478-111">針對屬於 Microsoft 365 群組或通訊網站的小組網站：</span><span class="sxs-lookup"><span data-stu-id="d9478-111">For a team site that belongs to an Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="d9478-112">這些新網站類型與整個組織設定具有相同的共用設定，除非整個組織設定允許使用不需要登入的連結來共用檔案。</span><span class="sxs-lookup"><span data-stu-id="d9478-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="d9478-113">在此情況下，網站允許與新的和現有的外部使用者共用登入。</span><span class="sxs-lookup"><span data-stu-id="d9478-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="d9478-114">若要變更特定網站的設定，請使用新 SharePoint 系統管理中心或 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="d9478-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="d9478-115">[深入了解](https://go.microsoft.com/fwlink/?linkid=871863)。</span><span class="sxs-lookup"><span data-stu-id="d9478-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="d9478-116">任何網站的外部共用設定，都比整個組織的設定更具限制性，但不如整個組織的設定。</span><span class="sxs-lookup"><span data-stu-id="d9478-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

