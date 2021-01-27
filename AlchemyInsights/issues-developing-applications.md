---
title: 開發應用程式的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950690"
---
# <a name="issues-developing-applications"></a>開發應用程式的問題

若要針對建立 Azure Active Directory (AD) 應用程式時最常見的問題進行疑難排解，請參閱下列文章：

- [我只有在使用 Chrome 網頁瀏覽器登入應用程式時會發生問題](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [我不知道如何變更應用程式的權杖生命週期預設值](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [我對於應用程式同意的運作方式感到困惑](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [我不知道如何將權限授與我的應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [我不了解委派和應用程式權限之間的差異](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory 驗證程式庫 (ADAL) 和 Azure AD Graph API (AAD Graph) 的終止支援** _

- 從 2020 年 6 月 30 日起，我們不再將任何新功能新增至 Azure Active Directory 驗證程式庫 (ADAL) 和 Azure AD Graph API (AAD Graph)。 我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。

- 從 2022 年 6 月 30 日起，我們將終止 ADAL 和 AAD Graph 的支援，並不再提供技術支援或安全性更新。 由於此情況，以下是一些影響：

    - 在現有作業系統版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會取得任何技術支援或安全性更新。

    - 在此時間之後使用 AAD Graph 的應用程式可能無法再收到 AAD Graph 端點的回應

_ *ADAL 移轉**

如果您使用 Microsoft 應用程式，建議您更新至 Microsoft 驗證程式庫 (MSAL)，其包含最新的功能和安全性更新。 本建議是由 Microsoft 在終止支援期限之前起始將其應用程式移轉至 MSAL 的程序。 

Microsoft 將其應用程式移轉至 MSAL，可確保應用程式能夠從 MSAL 持續的安全性與功能增強中受益。

1. [閱讀 ADAL 常見問題集](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [了解如何以每個平台為基礎移轉應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. 如果您需要協助了解您的哪些應用程式使用 ADAL，建議您檢閱所有應用程式的原始程式碼，並且 (如適用) 向任何獨立軟體廠商 (ISV) 或應用程式提供者諮詢。 Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。

**AAD Graph 移轉**

針對使用 AAD Graph 的應用程式，請依照我們的指導方針，將 AAD Graph 應用程式移轉至 Microsoft Graph：

1. [我們的移轉檢查清單可做為起點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
2. 您的 Azure 應用程式註冊入口網站會顯示哪些應用程式正在使用 AAD Graph。 建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何獨立軟體廠商 (ISV) 或應用程式提供者諮詢。 Microsoft 支援服務也可為您提供租用戶中所有 AAD Graph 使用狀況的資訊。







