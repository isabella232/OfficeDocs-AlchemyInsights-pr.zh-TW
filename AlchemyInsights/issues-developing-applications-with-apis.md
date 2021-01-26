---
title: 使用 APIs 來開發應用程式的問題
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951873"
---
# <a name="issues-developing-applications-with-apis"></a>使用 APIs 來開發應用程式的問題

若要開始使用 Azure Active Directory Graph API，請參閱 [AZURE Ad GRAPH api 快速入門手冊](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ，或查看 [互動式 AZURE ad graph api 參考檔](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)。

**Azure Active Directory 驗證程式庫的支援終止 (ADAL) 和 Azure AD Graph API (AAD Graph)**

**從2020年6月30日起**，我們將不再將任何新功能新增至 ADAL 和 Azure AD Graph。 我們將繼續提供技術支援和安全性更新，但不會再提供功能更新。

**從2022年6月30日起**，我們將結束支援 ADAL 和 Azure AD Graph，而且將不再提供技術支援或安全性更新。

在此時間之後，使用 ADAL 的現有作業系統版本的應用程式仍可運作，但不會取得任何技術支援或安全性更新。

在此時間之後使用 Azure AD Graph 的應用程式可能不再接收 Azure AD Graph 端點的回應。

**ADAL 遷移**

建議您更新至 [Microsoft 驗證程式庫 (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)，其具有最新的功能和安全性更新。

如果您使用的是 Microsoft 應用程式，請知道 Microsoft 正在將其應用程式遷移至 MSAL 的程式，以在支援的期限內進行遷移，以確保他們能夠從 MSAL 的持續安全性和功能改進中受益。

1. [閱讀 ADAL 常見問題解答](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. [瞭解如何以每個平臺為基礎遷移應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)。
1. 如果您需要協助瞭解您使用 ADAL 的應用程式，建議您檢查您的所有應用程式原始程式碼，並在適用時，向內送出任何 Isv 或應用程式提供者。 Microsoft 支援也可以提供您租使用者中所有非 Microsoft ADAL 應用程式的清單。

**AAD 圖形遷移**

針對使用 Azure AD Graph 的應用程式，請遵循我們的指導，將 [AZURE AD Graph 應用程式遷移至 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)。

1. [我們的遷移檢查清單提供開始點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。 
1. Azure 應用程式註冊入口網站會顯示哪些應用程式使用 AAD Graph。 我們建議您檢查您的所有應用程式原始程式碼，並在適用時，向內送出任何 Isv 或應用程式提供者。 Microsoft 支援也可以提供您租使用者中所有 AAD 圖形使用方式的清單。
1. 若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。 [Microsoft graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true)會列出與每個主要 Microsoft Graph APIs 集合相關聯的許可權。 此外，它也提供如何使用許可權的指導方針。
