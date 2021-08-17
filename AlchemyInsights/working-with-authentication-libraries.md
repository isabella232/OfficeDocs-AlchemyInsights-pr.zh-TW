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
ms.openlocfilehash: b667e699e1595b21d80788123de13daffbe79a35b1671e9d35eaa6cd980693db
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083077"
---
# <a name="working-with-authentication-libraries"></a>使用驗證程式庫

若要解決 Microsoft 驗證程式庫 (MSAL) 的問題，請執行下列建議步驟：

1. **使用 MSAL**：[Microsoft 身分識別平台驗證程式庫](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) (部分機器翻譯) - 本文說明 Microsoft 驗證程式庫支援數個應用程式類型。 它包含程式庫原始程式碼；哪裡可以取得您應用程式專案的套件；以及程式庫是否支援使用者登入 (驗證)、存取受保護的 Web API (授權) 或兩者皆支援。

2. **疑難排解驗證**：MSAL 支援數個驗證流程，以用於不同的應用程式案例。 根據您的用戶端應用程式建立方式，MSAL 可以使用 Microsoft 身分識別平台支援的一或多個驗證流程。 這些流程會產生數種類型的權杖和授權碼，並需要不同的權杖才能運作。

3. **存取權杖**：[Microsoft 身分識別平台存取權杖](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) (部分機器翻譯) - 了解 API 如何驗證和使用存取權杖內的宣告。 本文中的所有文件 (除非有說明)，僅適用於針對您註冊的 API 所發行的權杖。 它不適用於針對 Microsoft 擁有的 API 所發行的權杖，也無法使用這些權杖來驗證 Microsoft 身分識別平台如何針對您建立的 API 發行權杖。

**Azure Active Directory 驗證程式庫 (ADAL) 的終止支援**

- **從 2020 年 6 月 30 日起**，我們不再將任何新功能新增至 ADAL 和 Azure AD Graph。 我們會繼續提供技術支援和安全性更新，但將不再提供功能更新。
- **從 2022 年 6 月 30 日起**，我們將終止 ADAL 和 Azure AD Graph 的支援，並不再提供技術支援或安全性更新。
- 在現有作業系統版本上使用 ADAL 的應用程式將在此時間後繼續運作，但不會 *取得任何技術支援或安全性更新*。
- 在此時間之後，使用 Azure AD Graph 的應用程式可能無法再接收 Azure AD Graph 端點的回應。

**ADAL 遷移**

- 我們建議您更新至 MSAL，其中包含最新的功能和安全性更新。
- 如果您使用的是 Microsoft 應用程式，請了解 Microsoft 將於終止支援期限前將其應用程式遷移到 MSAL，確保這些應用程式將受益於 MSAL 持續的安全性與功能改進。

1. [閱讀 ADAL 常見問題集](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) (部分機器翻譯)。
2. [了解如何在每個平台上遷移應用程式](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance) (部分機器翻譯)。
3. 如果您在閱讀應用程式平台的指南之後，有其他問題，可以在 [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) 上貼上標籤 [azure-ad-adal-deprecation]，或在程式庫的 GitHub 存放庫中開啟問題。 請參閱 **MSAL 概觀** 文章章節中的 [語言和架構](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) (部分機器翻譯)，連結至每個程式庫的存放庫。
4. **如果您需要協助了解您的哪些應用程式使用 ADAL**，我們建議您檢閱所有應用程式的原始程式碼。 如果適用，請連絡任何獨立軟體廠商 (ISV) 或應用程式提供者。 Microsoft 支援服務也可提供您租用戶中所有非 Microsoft ADAL 應用程式清單。







