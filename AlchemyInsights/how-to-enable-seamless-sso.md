---
title: 如何啟用無縫 SSO
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
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: d203c1256785a99426503a5386935d78f8966a8b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384672"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="a07eb-102">如何啟用無縫 SSO</span><span class="sxs-lookup"><span data-stu-id="a07eb-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="a07eb-103">透過[AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)啟用無縫 SSO。</span><span class="sxs-lookup"><span data-stu-id="a07eb-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="a07eb-104">如果您要進行 Azure AD Connect 的全新安裝, 請選擇[自訂安裝路徑](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)。</span><span class="sxs-lookup"><span data-stu-id="a07eb-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="a07eb-105">在 [**使用者登入**] 頁面上, 選擇 [**啟用單一登入**] 選項。</span><span class="sxs-lookup"><span data-stu-id="a07eb-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="a07eb-106">若要確認您是否已正確啟用有效 SSO:</span><span class="sxs-lookup"><span data-stu-id="a07eb-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="a07eb-107">以全域系統管理員身分登入[Azure Active Directory 系統管理中心](https://aad.portal.azure.com)。</span><span class="sxs-lookup"><span data-stu-id="a07eb-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="a07eb-108">在左窗格中選取 [ **Azure Active Directory** ]。</span><span class="sxs-lookup"><span data-stu-id="a07eb-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="a07eb-109">確認**已啟用**無縫單一登入。</span><span class="sxs-lookup"><span data-stu-id="a07eb-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="a07eb-110">若要深入瞭解, 請參閱[Azure Active Directory 無縫單一登入: 快速入門](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。</span><span class="sxs-lookup"><span data-stu-id="a07eb-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  