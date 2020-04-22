---
title: ADFS 同盟憑證到期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710398"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="21836-102">ADFS 同盟憑證到期</span><span class="sxs-lookup"><span data-stu-id="21836-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="21836-103">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="21836-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="21836-104">在電腦上安裝 Windows PowerShell 的 Microsoft Azure Active Directory 模組（如果尚未安裝模組）。</span><span class="sxs-lookup"><span data-stu-id="21836-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="21836-105">若要這麼做，請移至[使用 Windows PowerShell 管理 AZURE AD](https://aka.ms/aadposh)。</span><span class="sxs-lookup"><span data-stu-id="21836-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="21836-106">請遵循「案例1： AD FS 權杖簽署憑證已過期」一節中的「案例」[當同盟使用者登入 Microsoft 365、Azure 或 Intune 時，「存取網站時發生問題](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)」一節。</span><span class="sxs-lookup"><span data-stu-id="21836-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Microsoft 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="21836-107">依照[更新或修復 Microsoft、Azure 或 Intune 中](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)的同盟網域的設定中的步驟進行。</span><span class="sxs-lookup"><span data-stu-id="21836-107">Follow the steps in [Update or repair the settings of a federated domain in Microsoft, Azure, or Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).</span></span>

    <span data-ttu-id="21836-108">若要深入瞭解如何更新同盟憑證，請參閱[更新 Microsoft 365 和 Azure Active Directory 的同盟憑證](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="21836-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Microsoft 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
