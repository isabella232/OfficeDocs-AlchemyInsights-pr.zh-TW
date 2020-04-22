---
title: 您的其中一個內部部署同盟服務憑證已過期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761374"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="3c260-102">您的其中一個內部部署同盟服務憑證已過期</span><span class="sxs-lookup"><span data-stu-id="3c260-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="3c260-103">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="3c260-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="3c260-104">在電腦上安裝 Windows PowerShell 的 Microsoft Azure Active Directory 模組（如果尚未安裝模組）。</span><span class="sxs-lookup"><span data-stu-id="3c260-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="3c260-105">若要這麼做，請移至[Azure Active Directory PowerShell 的圖形](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="3c260-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="3c260-106">請遵循「案例1： AD FS 權杖簽署憑證已到期」一節中的「[當同盟使用者登入 Office 365、Azure 或 Intune 時，存取網站時發生問題](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)」一節。</span><span class="sxs-lookup"><span data-stu-id="3c260-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="3c260-107">請遵循 t-sql 中的步驟，以在[Office 365、Azure 或 Intune 中更新或修復同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)。</span><span class="sxs-lookup"><span data-stu-id="3c260-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="3c260-108">如需有關如何更新同盟憑證的詳細資訊，請參閱[用於 O365 和 AZURE AD 的憑證更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="3c260-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

