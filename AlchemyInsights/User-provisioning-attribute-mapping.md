---
title: 使用者佈建屬性對應
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/22/2021
ms.locfileid: "49935347"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="c3515-102">使用者佈建屬性對應</span><span class="sxs-lookup"><span data-stu-id="c3515-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="c3515-103">若要疑難排解已知的屬性對應問題，請參閱[屬性對應](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)。</span><span class="sxs-lookup"><span data-stu-id="c3515-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="c3515-104">Microsoft Azure Active Directory (AD) 可支援將使用者佈建提供給協力廠商 SaaS 應用程式 (例如 Salesforce、G Suite 及其他)。</span><span class="sxs-lookup"><span data-stu-id="c3515-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="c3515-105">如果您為某個協力廠商 SaaS 應用程式啟用使用者佈建，Azure 入口網站會透過屬性對應來控制其屬性值。</span><span class="sxs-lookup"><span data-stu-id="c3515-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="c3515-106">若要了解如何自訂預設的屬性對應，請參閱[在 Azure Active Directory 中為 SaaS 應用程式自訂使用者佈建屬性對應](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)。</span><span class="sxs-lookup"><span data-stu-id="c3515-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="c3515-107">若要深入了解 SaaS 應用程式使用者佈建，請參閱[什麼是在 Azure AD 中自動佈建 SaaS 應用程式使用者？](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="c3515-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="c3515-108">為使用者佈建自訂屬性對應時，您可能會發現您要對應的屬性並未出現在來源屬性清單中。</span><span class="sxs-lookup"><span data-stu-id="c3515-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="c3515-109">[將屬性從內部部署 Active Directory 同步處理至 Azure AD 以佈建至應用程式](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)文章說明如何透過將屬性從內部部署 AD 同步處理到 Azure AD，藉此新增遺漏的屬性。</span><span class="sxs-lookup"><span data-stu-id="c3515-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
