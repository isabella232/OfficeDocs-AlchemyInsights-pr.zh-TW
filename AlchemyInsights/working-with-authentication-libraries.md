---
title: 使用驗證程式庫
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897492"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="ecacd-102">使用驗證程式庫</span><span class="sxs-lookup"><span data-stu-id="ecacd-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="ecacd-103">若要解決 Microsoft 驗證程式庫 (MSAL) 的問題，請執行下列建議步驟：</span><span class="sxs-lookup"><span data-stu-id="ecacd-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="ecacd-104">**使用 MSAL**：[Microsoft 身分識別平台驗證程式庫](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (部分機器翻譯) - 本文說明 Microsoft 驗證程式庫支援數個應用程式類型。</span><span class="sxs-lookup"><span data-stu-id="ecacd-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="ecacd-105">它包含程式庫原始程式碼；哪裡可以取得您應用程式專案的套件；以及程式庫是否支援使用者登入 (驗證)、存取受保護的 Web API (授權) 或兩者皆支援。</span><span class="sxs-lookup"><span data-stu-id="ecacd-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="ecacd-106">**疑難排解驗證**：MSAL 支援數個驗證流程，以用於不同的應用程式案例。</span><span class="sxs-lookup"><span data-stu-id="ecacd-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="ecacd-107">根據您的用戶端應用程式建立方式，MSAL 可以使用 Microsoft 身分識別平台支援的一或多個驗證流程。</span><span class="sxs-lookup"><span data-stu-id="ecacd-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="ecacd-108">這些流程會產生數種類型的權杖和授權碼，並需要不同的權杖才能運作。</span><span class="sxs-lookup"><span data-stu-id="ecacd-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="ecacd-109">**存取權杖**：[Microsoft 身分識別平台存取權杖](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) (部分機器翻譯) - 了解 API 如何驗證和使用存取權杖內的宣告。</span><span class="sxs-lookup"><span data-stu-id="ecacd-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="ecacd-110">本文中的所有文件 (除非有說明)，僅適用於針對您註冊的 API 所發行的權杖。</span><span class="sxs-lookup"><span data-stu-id="ecacd-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="ecacd-111">它不適用於針對 Microsoft 擁有的 API 所發行的權杖，也無法使用這些權杖來驗證 Microsoft 身分識別平台如何針對您建立的 API 發行權杖。</span><span class="sxs-lookup"><span data-stu-id="ecacd-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="ecacd-112">**Azure Active Directory 驗證程式庫 (ADAL) 的終止支援**</span><span class="sxs-lookup"><span data-stu-id="ecacd-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="ecacd-113">**從 2020 年 6 月 30 日起**，我們不再將任何新功能新增至 ADAL 和 Azure AD Graph。</span><span class="sxs-lookup"><span data-stu-id="ecacd-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="ecacd-114">我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。</span><span class="sxs-lookup"><span data-stu-id="ecacd-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="ecacd-115">**從 2022 年 6 月 30 日起**，我們將終止 ADAL 和 Azure AD Graph 的支援，並不再提供技術支援或安全性更新。</span><span class="sxs-lookup"><span data-stu-id="ecacd-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="ecacd-116">在現有作業系統版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會 *取得任何技術支援或安全性更新*。</span><span class="sxs-lookup"><span data-stu-id="ecacd-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="ecacd-117">在此時間之後，使用 Azure AD Graph 的應用程式可能無法再接收 Azure AD Graph 端點的回應。</span><span class="sxs-lookup"><span data-stu-id="ecacd-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="ecacd-118">**ADAL 遷移**</span><span class="sxs-lookup"><span data-stu-id="ecacd-118">**ADAL Migration**</span></span>

- <span data-ttu-id="ecacd-119">我們建議您更新至 MSAL，其中包含最新的功能和安全性更新。</span><span class="sxs-lookup"><span data-stu-id="ecacd-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="ecacd-120">如果您使用的是 Microsoft 應用程式，請了解 Microsoft 將於終止支援期限前將其應用程式遷移到 MSAL，確保這些應用程式將受益於 MSAL 持續的安全性與功能改進。</span><span class="sxs-lookup"><span data-stu-id="ecacd-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="ecacd-121">[閱讀 ADAL 常見問題集](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="ecacd-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="ecacd-122">[了解如何在每個平台上遷移應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="ecacd-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="ecacd-123">如果您在閱讀應用程式平台的指南之後，有其他問題，可以在 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) 上貼上標籤 [azure-ad-adal-deprecation]，或在程式庫的 GitHub 存放庫中開啟問題。</span><span class="sxs-lookup"><span data-stu-id="ecacd-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="ecacd-124">請參閱 **MSAL 概觀** 文章章節中的[語言和架構](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) (部分機器翻譯)，連結至每個程式庫的存放庫。</span><span class="sxs-lookup"><span data-stu-id="ecacd-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="ecacd-125">**如果您需要協助了解您的哪些應用程式使用 ADAL**，我們建議您檢閱所有應用程式的原始程式碼。</span><span class="sxs-lookup"><span data-stu-id="ecacd-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="ecacd-126">如果適用，請連絡任何獨立軟體廠商 (ISV) 或應用程式提供者。</span><span class="sxs-lookup"><span data-stu-id="ecacd-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="ecacd-127">Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。</span><span class="sxs-lookup"><span data-stu-id="ecacd-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







