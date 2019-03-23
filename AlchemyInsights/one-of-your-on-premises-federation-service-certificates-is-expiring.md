---
title: 下列其中一個內部部署同盟服務憑證即將到期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: e1afad0bab317af0f60a6ebda8c3ec8be398e38d
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753021"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a><span data-ttu-id="f3093-102">下列其中一個內部部署同盟服務憑證即將到期</span><span class="sxs-lookup"><span data-stu-id="f3093-102">One of your on-premises Federation Service Certificates is expiring</span></span>

<span data-ttu-id="f3093-103">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="f3093-103">To resolve this issue, follow these steps:</span></span>
  
- <span data-ttu-id="f3093-104">（如果尚未安裝模組），請在電腦上安裝 Microsoft Azure Active Directory 的 Windows PowerShell 模組。</span><span class="sxs-lookup"><span data-stu-id="f3093-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="f3093-105">若要這麼做，請移至[Azure Active Directory PowerShell 的圖表](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="f3093-105">To do this, go to [Azure Active Directory PowerShell for Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)</span></span>
    
- <span data-ttu-id="f3093-106">請遵循的步驟 」 案例 1: AD FS 權杖簽署憑證過期 」] 區段中的[「 時發生問題，存取的網站 」 的錯誤，AD FS 的同盟的使用者登入 Office 365、 Azure 或 Intune 時](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。</span><span class="sxs-lookup"><span data-stu-id="f3093-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
- <span data-ttu-id="f3093-107">遵循 t[如何更新或修復 Office 365、 Azure 或 Intune 中的同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步驟。</span><span class="sxs-lookup"><span data-stu-id="f3093-107">Follow the steps in t[How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
<span data-ttu-id="f3093-108">如需更新同盟憑證的詳細資訊，請參閱 <<c0>的 O365 和 Azure AD 的憑證更新。</span><span class="sxs-lookup"><span data-stu-id="f3093-108">For more information about renewing Federation certificates, see [Certificate renewal for O365 and Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
  

