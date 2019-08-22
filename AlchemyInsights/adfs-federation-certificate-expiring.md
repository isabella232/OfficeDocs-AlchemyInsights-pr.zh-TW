---
title: ADFS 同盟憑證到期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: c9922258c2d203cc07c1a1055ffa36c23a756115
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36499882"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="5a476-102">ADFS 同盟憑證到期</span><span class="sxs-lookup"><span data-stu-id="5a476-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="5a476-103">若要解決此問題，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="5a476-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="5a476-104">（如果尚未安裝模組），請在電腦上安裝 Microsoft Azure Active Directory 的 Windows PowerShell 模組。</span><span class="sxs-lookup"><span data-stu-id="5a476-104">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed).</span></span> <span data-ttu-id="5a476-105">若要這麼做，請前往[管理使用 Windows PowerShell 的 Azure AD](https://aka.ms/aadposh)。</span><span class="sxs-lookup"><span data-stu-id="5a476-105">To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>

2. <span data-ttu-id="5a476-106">請遵循的步驟 」 案例 1: AD FS 權杖簽署憑證過期 」] 區段中的[「 時發生問題，存取的網站 」 的錯誤，AD FS 的同盟的使用者登入 Office 365、 Azure 或 Intune 時](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。</span><span class="sxs-lookup"><span data-stu-id="5a476-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>

3. <span data-ttu-id="5a476-107">請遵循[如何更新或修復 Office 365、 Azure 或 Intune 中的同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)步驟。</span><span class="sxs-lookup"><span data-stu-id="5a476-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>

    <span data-ttu-id="5a476-108">若要深入了解更新同盟憑證，請參閱[Office 365 和 Azure Active Directory 的續約同盟憑證](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。</span><span class="sxs-lookup"><span data-stu-id="5a476-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
