---
title: 932 升級 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 9add88a0e4a2590639cbfc546afdcdf5e6aa4886
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28279085"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="074ad-102">升級 Azure AD 連線</span><span class="sxs-lookup"><span data-stu-id="074ad-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="074ad-p101">預設會自動升級為啟用 Azure AD 連線，有助於確保您正在執行的最新版本。若要確認自動升級設定，請 Azure AD PowerShell 中使用**Get ADSyncAutoUpgrade**指令程式。此指令程式會傳回下列值之一：</span><span class="sxs-lookup"><span data-stu-id="074ad-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="074ad-106">**Enabled**： 啟用自動升級。</span><span class="sxs-lookup"><span data-stu-id="074ad-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="074ad-107">**停用**： 停用自動升級。</span><span class="sxs-lookup"><span data-stu-id="074ad-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="074ad-p102">**已擱置**： 系統已不再合格接收自動升級。您不能設定這個值 ；它是由系統設定。</span><span class="sxs-lookup"><span data-stu-id="074ad-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="074ad-110">如需詳細資訊，請參閱[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)。</span><span class="sxs-lookup"><span data-stu-id="074ad-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="074ad-111">若要下載最新版的 Azure AD 連線，請前往[https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594)。</span><span class="sxs-lookup"><span data-stu-id="074ad-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

