---
title: 'SAML 斷言 (權杖) '
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004341"
- "7753"
ms.openlocfilehash: 557e23da09df3ab066c2ad7c0352f5fd904b5490
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884566"
---
# <a name="saml-assertions-tokens"></a><span data-ttu-id="7a475-102">SAML 斷言 (權杖) </span><span class="sxs-lookup"><span data-stu-id="7a475-102">SAML Assertions (Tokens)</span></span>

1. <span data-ttu-id="7a475-103">安全性聲明標記語言 (SAML) token 是宣告的 XML 標記法。</span><span class="sxs-lookup"><span data-stu-id="7a475-103">Security Assertions Markup Language (SAML) tokens are XML representations of claims.</span></span> <span data-ttu-id="7a475-104">依預設，同盟安全性案例中 (WCF) 使用的 SAML 權杖 Windows Communication Foundation 是由發行的權杖使用。</span><span class="sxs-lookup"><span data-stu-id="7a475-104">By default, SAML tokens Windows Communication Foundation (WCF) uses in federated security scenarios are issued tokens.</span></span> <span data-ttu-id="7a475-105">如需詳細資訊，請參閱 [SAML 權杖和宣告](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims)。</span><span class="sxs-lookup"><span data-stu-id="7a475-105">For more information, see [SAML Tokens and Claims](https://docs.microsoft.com/dotnet/framework/wcf/feature-details/saml-tokens-and-claims).</span></span>
2. <span data-ttu-id="7a475-106">Microsoft identity 平臺會在處理每個驗證流程時發出多種類型的安全性權杖。</span><span class="sxs-lookup"><span data-stu-id="7a475-106">The Microsoft identity platform emits several types of security tokens in the processing of each authentication flow.</span></span> <span data-ttu-id="7a475-107">[Saml 權杖宣告參考](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) 說明 saml 2.0 token 的格式、安全性特性和內容。</span><span class="sxs-lookup"><span data-stu-id="7a475-107">[SAML token claims reference](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens) describes the format, security characteristics, and contents of SAML 2.0 tokens.</span></span>
3. <span data-ttu-id="7a475-108">遵循 [Microsoft identity 平臺的可設定權杖生命週期](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) 中的指導方針，以瞭解如何設定權杖存留期。</span><span class="sxs-lookup"><span data-stu-id="7a475-108">Follow the guidance in [Configurable token lifetimes in Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes) to understand how to configure token lifetimes.</span></span>
4. <span data-ttu-id="7a475-109">請依照 [本文](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) 所述的步驟，瞭解如何設定 AZURE AD SAML 權杖加密。</span><span class="sxs-lookup"><span data-stu-id="7a475-109">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/howto-saml-token-encryption) to understand how to configure Azure AD SAML token encryption.</span></span>
5. <span data-ttu-id="7a475-110">在 Azure AD 中，您可以設定憑證簽署選項和憑證簽署演算法。</span><span class="sxs-lookup"><span data-stu-id="7a475-110">In Azure AD, you can set up certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="7a475-111">如需詳細資訊，請參閱在 [Azure Active Directory 中的畫廊應用程式的 SAML 權杖中的「高級憑證簽署選項](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)」。</span><span class="sxs-lookup"><span data-stu-id="7a475-111">For more information, see [Advanced certificate signing options in the SAML token for gallery apps in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>
