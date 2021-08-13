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
ms.openlocfilehash: 73da476cc5913a16911839a59b80959d3c99a8bc22471febe421b022ce2c49ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53918134"
---
# <a name="user-provisioning-attribute-mapping"></a>使用者佈建屬性對應

1. 若要疑難排解已知的屬性對應問題，請參閱[屬性對應](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings)。 
2. Microsoft Azure Active Directory (AD) 可支援將使用者佈建提供給協力廠商 SaaS 應用程式 (例如 Salesforce、G Suite 及其他)。 如果您為某個協力廠商 SaaS 應用程式啟用使用者佈建，Azure 入口網站會透過屬性對應來控制其屬性值。 若要了解如何自訂預設的屬性對應，請參閱[在 Azure Active Directory 中為 SaaS 應用程式自訂使用者佈建屬性對應](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes)。
    - 若要深入了解 SaaS 應用程式使用者佈建，請參閱[什麼是在 Azure AD 中自動佈建 SaaS 應用程式使用者？](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning) 
3. 為使用者佈建自訂屬性對應時，您可能會發現您要對應的屬性並未出現在來源屬性清單中。 [將屬性從內部部署 Active Directory 同步處理至 Azure AD 以佈建至應用程式](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping)文章說明如何透過將屬性從內部部署 AD 同步處理到 Azure AD，藉此新增遺漏的屬性。
