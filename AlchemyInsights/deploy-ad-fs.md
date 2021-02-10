---
title: 部署 AD FS
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
- "1300012"
- "7420"
ms.openlocfilehash: a304504f7483036884878639dfa6ebfc3cdfcac8
ms.sourcegitcommit: 05a9dd3121c21322dc9ddec4c2eec548cafd5a43
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/09/2021
ms.locfileid: "50165244"
---
# <a name="deploy-ad-fs"></a><span data-ttu-id="0615b-102">部署 AD FS</span><span class="sxs-lookup"><span data-stu-id="0615b-102">Deploy AD FS</span></span>

<span data-ttu-id="0615b-103">Active Directory Federation Services (AD FS) 部署使用您的內部部署基礎結構來驗證 Office 365 服務的使用者。</span><span class="sxs-lookup"><span data-stu-id="0615b-103">An Active Directory Federation Services (AD FS) deployment uses your on-premises infrastructure to authenticate users for ‎Office 365 services.</span></span> <span data-ttu-id="0615b-104">透過同盟登入，您可以讓使用者登入 Office 365 服務和軟體成為服務 (SAAS) 與 Azure Active Directory (Azure AD) 整合的應用程式。</span><span class="sxs-lookup"><span data-stu-id="0615b-104">With federated sign-in, you can enable users to sign in to Office 365 services and Software as a Service (SAAS) applications that are integrated with Azure Active Directory (Azure AD).</span></span> <span data-ttu-id="0615b-105">同盟登入會透過 AD FS 向內部部署 Active Directory 驗證使用者。</span><span class="sxs-lookup"><span data-stu-id="0615b-105">Federated sign-in authenticates users against your on-premises Active Directory via AD FS.</span></span> <span data-ttu-id="0615b-106">此外，在公司網路上，使用者不需要重新輸入密碼。</span><span class="sxs-lookup"><span data-stu-id="0615b-106">Also, while on the corporate network, users won't be required to reenter their passwords.</span></span>

<span data-ttu-id="0615b-107">[AD FS 部署顧問](https://go.microsoft.com/fwlink/?linkid=2071178)為您提供部署內部部署 AD FS 基礎結構的逐步指引，該基礎結構可驗證 Microsoft 365 和 Office 365 服務的使用者。</span><span class="sxs-lookup"><span data-stu-id="0615b-107">The [AD FS deployment advisor](https://go.microsoft.com/fwlink/?linkid=2071178) provides you with step-by-step guidance on deploying an on-premises AD FS infrastructure that authenticates users for Microsoft 365 and Office 365 services.</span></span> <span data-ttu-id="0615b-108">透過本指南，您的組織可以查看 AD FS 元件和需求、取得及安裝部署所需的 SSL 憑證，以及安裝必要的 web 應用程式 proxy 伺服器。</span><span class="sxs-lookup"><span data-stu-id="0615b-108">With this guide, your organization can review AD FS components and requirements, acquire and install SSL certificates that are necessary for deployment, and install a required web application proxy server.</span></span>
