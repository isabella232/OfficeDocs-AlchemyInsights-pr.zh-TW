---
title: 讓使用者能夠存取 SharePoint 和 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677198"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="71763-102">讓使用者能夠存取 SharePoint 和 OneDrive</span><span class="sxs-lookup"><span data-stu-id="71763-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="71763-103">如果有 OneDrive 或 SharePoint 網站無法供先前具有存取權的使用者使用，則可能會發生暫時的服務問題。</span><span class="sxs-lookup"><span data-stu-id="71763-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="71763-104">檢查服務健康情況儀表板</span><span class="sxs-lookup"><span data-stu-id="71763-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="71763-105">如果您想讓組織中的人員能夠登入和使用 SharePoint 和 OneDrive，您必須為他們新增帳戶，並確定他們擁有授權，可讓他們存取 SharePoint 和 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="71763-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="71763-106">新增使用者的最簡單方法是在 Microsoft 365 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="71763-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="71763-107">移至 [Microsoft 365 系統管理中心中](https://portal.office.com/adminportal/home#/users)的 [作用中使用者] 頁面，然後按一下 [ **新增使用者**]。</span><span class="sxs-lookup"><span data-stu-id="71763-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="71763-108">填入使用者的資訊，並確定已選取 [ **產品授權**] 底下的 [授權]，並選取 [ **SharePoint 線上** ]。</span><span class="sxs-lookup"><span data-stu-id="71763-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="71763-109">請注意，如果您在組織中允許外部共用，使用者可以與組織外部的人員共用 SharePoint 和 OneDrive 內容。</span><span class="sxs-lookup"><span data-stu-id="71763-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="71763-110">您不需要授與這些外部使用者授權。</span><span class="sxs-lookup"><span data-stu-id="71763-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="71763-111">您也不需要為其新增帳戶，除非 [共用] 設為「只有現有的外部使用者」。</span><span class="sxs-lookup"><span data-stu-id="71763-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="71763-112">在此情況下，如果人員不在您組織的目錄中，您必須在 Azure AD 系統管理中心中將其新增為來賓使用者。</span><span class="sxs-lookup"><span data-stu-id="71763-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

