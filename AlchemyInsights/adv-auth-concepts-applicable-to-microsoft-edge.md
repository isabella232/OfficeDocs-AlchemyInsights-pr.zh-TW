---
title: 適用于 Microsoft Edge 的高級驗證概念
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398544"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="e469e-102">適用于 Microsoft Edge 的高級驗證概念</span><span class="sxs-lookup"><span data-stu-id="e469e-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="e469e-103">以下是適用于 Microsoft Edge 的高級驗證概念：</span><span class="sxs-lookup"><span data-stu-id="e469e-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="e469e-104">**主動驗證**</span><span class="sxs-lookup"><span data-stu-id="e469e-104">**Proactive Authentication**</span></span>

<span data-ttu-id="e469e-105">當您啟用 [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) 原則時，microsoft Edge 會嘗試透過 Microsoft 服務主動驗證已登入的使用者。</span><span class="sxs-lookup"><span data-stu-id="e469e-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="e469e-106">以固定的間隔，它會使用線上服務檢查是否有包含管理主動驗證的更新資訊清單。</span><span class="sxs-lookup"><span data-stu-id="e469e-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="e469e-107">好處：主動型驗證可讓驗證成為重要服務，例如 Office 新的 [索引標籤] 頁面。</span><span class="sxs-lookup"><span data-stu-id="e469e-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="e469e-108">此外，如果使用 Bing 做為搜尋引擎，事前驗證會提升位址列的效能，並協助產生針對您的業務需求個人化的搜尋結果。</span><span class="sxs-lookup"><span data-stu-id="e469e-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="e469e-109">**適用于 NTLM 驗證的 Windows Hello CredUI**</span><span class="sxs-lookup"><span data-stu-id="e469e-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="e469e-110">若在網站嘗試透過 NTLM 或協商機制登入使用者時，無法使用單一登入 (SSO) ，此功能可讓使用者與網站共用作業系統認證，以及使用 Windows Hello 身分驗證使用者介面來滿足驗證質詢。</span><span class="sxs-lookup"><span data-stu-id="e469e-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="e469e-111">此登入流程只會出現在 Windows 10 中，而且只有在 NTLM 或協商質詢中未取得 SSO 的使用者才會出現。</span><span class="sxs-lookup"><span data-stu-id="e469e-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="e469e-112">**使用儲存的密碼自動登入**</span><span class="sxs-lookup"><span data-stu-id="e469e-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="e469e-113">在 Microsoft Edge 中儲存密碼的使用者可以啟用自動登入已儲存認證的網站。</span><span class="sxs-lookup"><span data-stu-id="e469e-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="e469e-114">使用者可以在 edge://settings/passwords 中開啟或關閉此功能，也可以在 [密碼管理員](https://go.microsoft.com/fwlink/?linkid=2134622) 原則中加以設定。</span><span class="sxs-lookup"><span data-stu-id="e469e-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
