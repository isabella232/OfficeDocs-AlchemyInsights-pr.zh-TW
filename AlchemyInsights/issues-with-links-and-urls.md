---
title: 連結和 URL 的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7720"
- "9004329"
ms.openlocfilehash: 24885d873d6471a72ae66581ad1ceb0a19b664f7
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/25/2021
ms.locfileid: "49950687"
---
# <a name="issues-with-links-and-urls"></a>連結和 URL 的問題

重新導向 URI/回覆 URL (這兩個表示可互換) 是 Microsoft 身分識別平台用來傳回應用程式要求權杖的 URL。 如需這些 URL 的相關資訊，請參閱下列文章：

- [驗證流程和應用程式案例](https://docs.microsoft.com/azure/active-directory/develop/authentication-flows-app-scenarios) - 每個案例的 [應用程式註冊 **]** 頁面中重新導向 URI 的相關資訊。
- [重新導向 URI/回覆 URL 限制和限制](https://docs.microsoft.com/azure/active-directory/develop/reply-url)

**我不知道如何為我的應用程式註冊正確的重新導向 URI/回覆 URL**

使用您正在開發的應用程式登入時，如果登入對話方塊顯示 **AADSTS50011：要求中指定的回覆 URL 與為應用程式 <your app ID> 設定的回覆 URL 不符**，您需要將您的程式碼在對 Microsoft 身分識別平台的權杖要求中使用的重新導向 URI 新增至您的應用程式註冊。

若要新增回覆 URL，請移至 Azure 入口網站中 [應用程式註冊 **]** 頁面中的 [驗證 **]** 索引標籤，然後在 [重新導向 URI **]** 區段中新增項目。 重新導向 URI 需區分類型 (Web 或行動裝置/傳統型)。 您需要輸入的值取決於您正在建立的應用程式類型，如下所述：

- 針對單一頁面應用程式和 Web應用程式，則回覆 URL 是您應用程式中的 URL。 請參閱[單一頁面應用程式註冊](https://docs.microsoft.com/azure/active-directory/develop/scenario-spa-app-registration#register-a-redirect-uri)或[使用 Azure 入口網站註冊 Web 應用程式](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration?tabs=aspnetcore#register-an-app-using-azure-portal)
- 針對傳統型應用程式，您需要選擇的值取決於：
    - 平台 (MacOS 與 Windows 或 Linux 不同)
    - 取得權杖的方式 (互動式、使用裝置代碼流程、使用整合式 Windows 驗證 [IWA] 或使用使用者名稱/密碼)。
    如需詳細資訊，請參閱[傳統型應用程式 - 應用程式註冊 - 重新導向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-desktop-app-registration#redirect-uris)
- 針對行動裝置應用程式，重新導向 URI 取決於：
    - 平台 (iOS/Android/UWP)
    - 用來建立您的應用程式的資訊，例如 iOS 中的組建識別碼，以及 Android 上的套件名稱和簽名雜湊。Azure 入口網站應用程式註冊將協助您。 如需詳細資訊，請參閱[平台設定和重新導向 URI](https://docs.microsoft.com/azure/active-directory/develop/scenario-mobile-app-registration#platform-configuration-and-redirect-uris)。

> [!NOTE]
> Web API 和某些取得權杖的無訊息方式 (IWA 和使用者名稱/密碼) 不需要重新導向 URI。

**我已部署我的 Web 應用程式，當我測試部署的應用程式時，收到回覆 URL 不相符的訊息**

為您要部署 Web 應用程式的所有位置新增重新導向 URI。 如需詳細資訊，請參閱[使用 Azure 入口網站註冊 Web 應用程式](https://docs.microsoft.com/azure/active-directory/develop/scenario-web-app-sign-user-app-registration)。

> [!NOTE]
> 在該位置部署應用程式之後，立即為該位置新增重新導向 URI。

**我無法註冊足夠數量的回覆 URL**

您是 ISV，您的每個客戶都有一或多個重新導向 URI。 您想要從 ADAL/Azure AD v1.0 移轉到 MSAL/Microsoft 身分識別平台，並且您達到[重新導向 URI 的數量上限](https://docs.microsoft.com/azure/active-directory/develop/reply-url#maximum-number-of-redirect-uris)。 若要解決此問題，請[將重新導向 URI 新增至與每個客戶對應的服務主體](https://docs.microsoft.com/azure/active-directory/develop/reply-url#add-redirect-uris-to-service-principals)。
