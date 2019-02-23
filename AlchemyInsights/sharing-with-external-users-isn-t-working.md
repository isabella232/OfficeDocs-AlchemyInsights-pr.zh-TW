---
title: 與外部使用者共用也無法正常運作
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 5/18/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 4b132a3cb0fac015ab44a1fa08565af15b7e8121
ms.sourcegitcommit: c003a5db7edc3a44fb5b31b46cd45f12b62d172a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/22/2019
ms.locfileid: "30207676"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="31ec8-102">修正問題與外部使用者共用 SharePoint 內容</span><span class="sxs-lookup"><span data-stu-id="31ec8-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="31ec8-103">請確定外部共用您的組織已開啟：</span><span class="sxs-lookup"><span data-stu-id="31ec8-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="31ec8-104">移至 [[服務&amp;增益集] 頁面上的 Microsoft 365 系統管理中心](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)，並按一下 [**網站**]。</span><span class="sxs-lookup"><span data-stu-id="31ec8-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="31ec8-p101">確定設定開啟以 「 開啟 」。如果已選取 「 唯一現有外部使用者 」，請確認外部使用者會列於 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="31ec8-p101">Make sure the setting is turned to "On." If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="31ec8-p102">確定外部共用其開啟網站。傳統的網站集合：</span><span class="sxs-lookup"><span data-stu-id="31ec8-p102">Make sure external sharing it turned on for the site. For a classic site collection:</span></span>
  
1. <span data-ttu-id="31ec8-109">在傳統 SharePoint 系統管理中心，在左窗格中，按一下 [**網站集合**]。</span><span class="sxs-lookup"><span data-stu-id="31ec8-109">In the classic SharePoint admin center, in the left pane, click **site collections**.</span></span>
    
2. <span data-ttu-id="31ec8-110">選取網站] 或 [網站]，並在功能區] 上按一下 [**共用**]。</span><span class="sxs-lookup"><span data-stu-id="31ec8-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="31ec8-111">Office 365] 群組中，屬於小組網站或通訊網站：</span><span class="sxs-lookup"><span data-stu-id="31ec8-111">For a team site that belongs to an Office 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="31ec8-p103">這些新的網站類型具有相同共用將設為您的整個組織的設定，除非整個組織的設定可讓共用檔案使用不需要登入的連結。在此例中，網站會允許共用與新的和現有外部使用者登入。若要變更特定網站的設定，請使用新的 SharePoint 系統管理中心 （預覽） 或 PowerShell。[解更多](https://go.microsoft.com/fwlink/?linkid=871863)。</span><span class="sxs-lookup"><span data-stu-id="31ec8-p103">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in. In this case, the sites allow sharing with new and existing external users who sign in. To change the setting for specific sites, use the new SharePoint admin center (preview) or PowerShell. [Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="31ec8-116">外部共用任何網站的設定可以更嚴格比在整個組織設定，但不是更寬鬆比全組織設定。</span><span class="sxs-lookup"><span data-stu-id="31ec8-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

