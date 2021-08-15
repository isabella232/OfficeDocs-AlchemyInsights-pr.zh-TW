---
title: Microsoft Graph API 問題
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975884"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API 問題

本主題也適用于仍在使用 Azure AD Graph API 的開發人員。 不過，**強烈** 建議您針對所有目錄、身分識別和存取管理案例使用 Microsoft Graph。

**驗證或授權問題**

- 如果您的應用程式 **無法取得標記** 以撥打 Microsoft Graph，請選擇 **取得存取權杖 (驗證)** Microsoft Graph 類別，以取得更多特定的說明和支援，以取得本主題。
- 當呼叫 Microsoft Graph 時，如果您的應用程式 **收到401或403授權錯誤**，請選擇 [**取得存取權被拒絕] 錯誤 (授權)** Microsoft Graph API 類別，以取得更多特定的說明和支援此主題。

**我想要使用 Microsoft Graph，但不確定開始的位置**

- [Microsoft Graph 概觀](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph 中的身分識別與存取管理綜述](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [建立 Microsoft Graph 應用程式的快速入門](https://docs.microsoft.com/graph/)
- **microsoft Graph Explorer** -測試您租使用者或示範租使用者中的 Microsoft Graph APIs

**我想要使用 Microsoft Graph，但是它是否支援我需要的1.0 版目錄 APIs？**

Microsoft Graph 是目錄、身分識別和存取管理的建議 API。 不過，Azure AD Graph 和 Microsoft Graph 中的可能仍然有一些差距。 請參閱下列文章，這些文章會反白顯示最新的差異，以協助您選擇：

- [Azure AD Graph 和 Microsoft Graph 之間的資源類型差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph 之間的屬性差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph 之間的方法差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**我正在通話的 API 無法運作-我可以在哪裡進行其他測試？**

**microsoft Graph Explorer** -測試您租使用者或示範租使用者中的 microsoft Graph APIs，也請參閱 Microsoft Graph Explorer 中的 **範例查詢**。

**我的應用程式速度太慢，也遭到節流。我可以進行哪些改進？**

視您的案例而定，有許多選項可讓您的應用程式更具能力，在某些情況下，當您) 進行許多呼叫時，可能會降低服務 (的限制。

- [Microsoft Graph 最佳作法](https://docs.microsoft.com/graph/best-practices-concept)
- [批次處理要求](https://docs.microsoft.com/graph/json-batching)
- [透過增量查詢追蹤變更](https://docs.microsoft.com/graph/delta-query-overview)
- [透過 webhooks 取得變更的通知](https://docs.microsoft.com/graph/webhooks)
- [節流指導](https://docs.microsoft.com/graph/throttling)

**在哪裡可以找到錯誤和已知問題的詳細資訊？**

- [Microsoft Graph 錯誤回應資訊](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph 的已知問題](https://docs.microsoft.com/graph/known-issues)

**我可以在哪裡檢查服務可用性和線上狀態？**

可透過 microsoft Graph 存取之基礎服務的服務可用性和連線能力會影響 microsoft Graph 的整體可用性和效能。

- 若為 Azure Active Directory 服務健康情況，請檢查 [ [Azure 狀態] 頁面](https://azure.microsoft.com/status/)中列出的 [**安全性 + 身分識別** 服務] 狀態。
- 針對參與 Microsoft Graph 的 Office 服務，請檢查 [ [Office 服務健康情況] 儀表板](https://portal.office.com/adminportal/home#/servicehealth)中所列服務的狀態。

Microsoft Graph 授權錯誤可能是幾個不同問題的結果，大部分會產生401或403錯誤。 例如，下列各項會導致授權錯誤：

- 不正確的[存取權杖取得流程](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios) (部分機器翻譯)
- 設定錯誤的 [權限範圍](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) (部分機器翻譯)
- 缺少[同意](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) (部分機器翻譯)

***Azure Active Directory 驗證程式庫的支援終止 (ADAL) 和 Azure AD Graph API (AAD Graph)***

**從2020年6月30日起**，我們將不再將任何新功能新增至 ADAL 和 Azure AD Graph。 我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。

**從2022年6月30日起**，我們將結束對 ADAL 和 Azure AD Graph 的支援，並且不再提供技術支援或安全性更新。

在現有作業系統版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會 *取得任何技術支援或安全性更新*。

在此時間之後，使用 Azure AD Graph 的應用程式可能無法再接收 Azure AD Graph 端點的回應。

**ADAL 遷移**

我們建議您更新至 [Microsoft 驗證程式庫 (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview) (部分機器翻譯)，其中包含最新的功能和安全性更新。

如果您使用的是 Microsoft 應用程式，請知道 Microsoft 正在將其應用程式遷移至 MSAL 的程式，以在支援的期限內進行遷移，以確保他們能夠從 MSAL 的持續安全性和功能改進中受益。

1. [閱讀 ADAL 常見問題集](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [了解如何以每個平台為基礎移轉應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. 如果您需要協助瞭解您使用 ADAL 的應用程式，建議您檢查您的所有應用程式原始程式碼，並在適用時，向內送出任何 Isv 或應用程式提供者。 Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。

**AAD Graph 移轉**

針對使用 Azure AD Graph 的應用程式，請遵循我們的指導，將[Azure ad Graph 應用程式遷移至 Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)。

1. [我們的移轉檢查清單可做為起點](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)。
2. 您的 Azure 應用程式註冊入口網站顯示哪些應用程式正在使用 AAD Graph。 我們建議您檢閱所有應用程式的原始程式碼，如果適用的話，請向任何 ISV 或應用程式提供者諮詢。 Microsoft 支援也可以提供您租使用者中所有 AAD Graph 使用方式的清單。
3. 若要讓您的應用程式存取 Microsoft Graph 中的資料，使用者或系統管理員必須透過同意程式授與其正確的許可權。 [microsoft Graph 許可權參考](https://docs.microsoft.com/graph/permissions-reference)會列出與每一組主要 Microsoft Graph APIs 相關聯的許可權。 此外，它也提供如何使用許可權的指導方針。
