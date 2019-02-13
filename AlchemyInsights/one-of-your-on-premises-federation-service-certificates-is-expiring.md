---
title: 其中一個內部部署同盟服務憑證已過期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: bed33ba4d09fe4598c5e73eb21f0af1b7670f4c1
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29914391"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="50f53-102">其中一個內部部署同盟服務憑證已過期</span><span class="sxs-lookup"><span data-stu-id="50f53-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="50f53-103">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="50f53-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="50f53-p101">（如果尚未安裝模組） 的電腦上安裝 Microsoft Azure Active Directory 的 Windows PowerShell 模組。若要這樣做，請移至[Azure Active Directory PowerShell 圖表](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="50f53-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="50f53-106">請遵循的步驟"案例 1： AD FS 權杖簽署憑證過期"] 區段中的[「 時發生問題存取的網站 」 從 AD FS 同盟的使用者登入 Office 365、 Azure、 或 Intune 時的錯誤](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。</span><span class="sxs-lookup"><span data-stu-id="50f53-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="50f53-107">請遵循 t[如何更新或修復 Office 365、 Azure、 或 Intune 同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)步驟。</span><span class="sxs-lookup"><span data-stu-id="50f53-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="50f53-108">如需更新同盟憑證的詳細資訊，請參閱[O365 和 Azure AD 的憑證更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="50f53-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

