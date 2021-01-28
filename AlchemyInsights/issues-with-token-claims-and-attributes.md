---
title: 權杖宣告和屬性的問題
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029979"
---
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="3b5c0-102">權杖宣告和屬性的問題</span><span class="sxs-lookup"><span data-stu-id="3b5c0-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="3b5c0-103">**Update、configure 或 remove token 宣告**</span><span class="sxs-lookup"><span data-stu-id="3b5c0-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="3b5c0-104">使用 Azure Active Directory (Azure AD) ，您可以在授權的應用程式之後收到的回應權杖中， [為角色宣告自訂宣告類型](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) 。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="3b5c0-105">應用程式開發人員可以在其 Azure AD 應用程式中使用選用的宣告，在傳送至其應用程式的標記中指定要使用的宣告。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="3b5c0-106">如需詳細資訊，請參閱為 [您的應用程式提供選用的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="3b5c0-107">[使用 Azure Active Directory 設定應用程式的群組宣告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims)。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="3b5c0-108">若在您的應用程式中使用無縫單一登入，請參閱 [自訂宣告中在企業應用程式的 SAML 權杖中發出的宣告](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="3b5c0-109">**宣告屬性對應**</span><span class="sxs-lookup"><span data-stu-id="3b5c0-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="3b5c0-110">若要使用 PowerShell 來設定宣告對應原則，請參閱 [自訂承租人中的特定應用程式在標記中發出的宣告 (Preview) ](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="3b5c0-111">目錄架構擴充屬性提供一種方法，可將其他資料儲存在使用者物件及其他目錄物件（例如群組、租使用者詳細資料、服務主體）上的 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="3b5c0-112">只有使用者物件上的分機屬性可用於發出宣告給應用程式。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="3b5c0-113">[使用宣告中的目錄架構擴充屬性](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) 說明如何使用目錄架構擴充屬性，將使用者資料傳送至權杖宣告中的應用程式。</span><span class="sxs-lookup"><span data-stu-id="3b5c0-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="3b5c0-114">如需權杖宣告的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="3b5c0-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="3b5c0-115">存取權杖中的宣告</span><span class="sxs-lookup"><span data-stu-id="3b5c0-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="3b5c0-116">Id_token 中的宣告</span><span class="sxs-lookup"><span data-stu-id="3b5c0-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="3b5c0-117">您可以期望的識別碼權杖和 Azure AD B2C 所發出之存取權杖的[宣告](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims)</span><span class="sxs-lookup"><span data-stu-id="3b5c0-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="3b5c0-118">SAML 權杖宣告參考</span><span class="sxs-lookup"><span data-stu-id="3b5c0-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
