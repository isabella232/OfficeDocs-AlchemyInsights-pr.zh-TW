---
title: 設定及疑難排解 SAML 宣告
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7799"
- "9004356"
ms.openlocfilehash: 306d2f451856a66f06447e3acd73e065da71cd64
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886798"
---
# <a name="configure-and-troubleshoot-saml-claims"></a><span data-ttu-id="80767-102">設定及疑難排解 SAML 宣告</span><span class="sxs-lookup"><span data-stu-id="80767-102">Configure and troubleshoot SAML claims</span></span>

<span data-ttu-id="80767-103">若要設定和疑難排解 SAML 宣告：</span><span class="sxs-lookup"><span data-stu-id="80767-103">To configure and troubleshoot SAML claims:</span></span>

1. <span data-ttu-id="80767-104">按照 [本文](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) 中概述的步驟，以設定企業應用程式的 SAML 權杖中發出的角色宣告。</span><span class="sxs-lookup"><span data-stu-id="80767-104">Follow the steps outlined in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) to configure the role claim issued in the SAML token for enterprise applications.</span></span>
2. <span data-ttu-id="80767-105">按照 [本文](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) 中的步驟，自訂企業應用程式的 SAML 權杖中發出的宣告。</span><span class="sxs-lookup"><span data-stu-id="80767-105">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization) to customize claims issued in the SAML token for enterprise applications.</span></span>
3. <span data-ttu-id="80767-106">按照 [本文](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) 中的步驟，自訂租用戶中特定應用程式的權杖所發出的宣告。</span><span class="sxs-lookup"><span data-stu-id="80767-106">Follow the steps in [this article](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping) to customize claims emitted in tokens for a specific app in a tenant.</span></span>
4. <span data-ttu-id="80767-107">閱讀 [本文](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications)，瞭解如何在應用程式 Proxy 中使用宣告感知應用程式。</span><span class="sxs-lookup"><span data-stu-id="80767-107">Read [this article](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-for-claims-aware-applications) to understand working with claims-aware apps in Application Proxy.</span></span>