---
title: 疑難排解 (SSO) browser 問題的無縫單一登入
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9377"
ms.openlocfilehash: 507dc5a3bdc5f1bc27cf12865daf98df6c702827
ms.sourcegitcommit: f835aa80f2d85e9c0549be9395110377dba50f3d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530816"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-browser-issues"></a><span data-ttu-id="c219d-102">疑難排解 (SSO) browser 問題的無縫單一登入</span><span class="sxs-lookup"><span data-stu-id="c219d-102">Troubleshoot Seamless Single Sign-on (SSO) browser issues</span></span>

<span data-ttu-id="c219d-103">大多數使用者可以使用下列步驟解決其無縫 SSO 瀏覽器問題：</span><span class="sxs-lookup"><span data-stu-id="c219d-103">Most users are able to resolve their Seamless SSO browser issue using the steps below:</span></span>

1. <span data-ttu-id="c219d-104">請確定您的瀏覽器是最新的。</span><span class="sxs-lookup"><span data-stu-id="c219d-104">Make sure your browser is up-to-date.</span></span>
2. <span data-ttu-id="c219d-105">從您的瀏覽器中刪除 cookie，以移除不正確 SSO 會話，並嘗試再次登入。</span><span class="sxs-lookup"><span data-stu-id="c219d-105">Delete cookies from your browser to remove an invalid SSO session and try logging in again.</span></span>
3. <span data-ttu-id="c219d-106">請嘗試使用其他瀏覽器登入。</span><span class="sxs-lookup"><span data-stu-id="c219d-106">Try logging in using a different browser.</span></span>

<span data-ttu-id="c219d-107">**已知瀏覽器問題**</span><span class="sxs-lookup"><span data-stu-id="c219d-107">**Known Browser Issues**</span></span>

- <span data-ttu-id="c219d-108">在 Firefox 上，無法以私人瀏覽模式使用無縫 SSO。</span><span class="sxs-lookup"><span data-stu-id="c219d-108">Seamless SSO doesn't work in private browsing mode on Firefox.</span></span>
- <span data-ttu-id="c219d-109">開啟增強型保護模式時，Internet Explorer 無法使用無縫 SSO。</span><span class="sxs-lookup"><span data-stu-id="c219d-109">Seamless SSO doesn't work in Internet Explorer when Enhanced Protected mode is turned on.</span></span>
- <span data-ttu-id="c219d-110">在 Microsoft Edge (舊版) 中，無法以私人瀏覽模式使用無縫 SSO。</span><span class="sxs-lookup"><span data-stu-id="c219d-110">Seamless SSO doesn't work in private browsing mode on Microsoft Edge (legacy).</span></span>
- <span data-ttu-id="c219d-111">在 iOS 和 Android 的行動瀏覽器上無法使用無縫 SSO。</span><span class="sxs-lookup"><span data-stu-id="c219d-111">Seamless SSO doesn't work on mobile browsers on iOS and Android.</span></span>

<span data-ttu-id="c219d-112">無縫 SSO 可根據 Chromium，支援下一個版本的 Microsoft Edge，而且會以設計方式在 InPrivate 和來賓模式下運作。</span><span class="sxs-lookup"><span data-stu-id="c219d-112">Seamless SSO supports the next version of Microsoft Edge based on Chromium and it works in InPrivate and Guest mode by design.</span></span>

<span data-ttu-id="c219d-113">**諮詢**</span><span class="sxs-lookup"><span data-stu-id="c219d-113">**Advisory**</span></span>

<span data-ttu-id="c219d-114">若要提出功能要求或詢問有關無縫 SSO 的技術問題，請參閱 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span><span class="sxs-lookup"><span data-stu-id="c219d-114">To make feature requests or ask technical questions about Seamless SSO, see [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html)</span></span>
