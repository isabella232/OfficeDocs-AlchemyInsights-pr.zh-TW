---
title: 設定和自訂應用程式
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/29/2021
ms.locfileid: "50043978"
---
# <a name="configure-and-customize-applications"></a>設定和自訂應用程式

**設定應用程式**

1. [快速入門： Configure The Azure Active Directory 中的應用程式屬性 (AZURE AD) 租](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) 使用者顯示如何設定應用程式的某些屬性。
2. 為了協助整合您的應用程式與 Azure Active Directory，我們已開發 [一組教程](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) ，可引導您完成設定。
3. [如何設定應用程式 proxy 應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) 可協助您瞭解如何在 Azure AD 中設定應用程式 proxy 應用程式，以將內部部署應用程式公開至雲端。
4. [下載 PingAccess 並設定您的應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)：遵循 *configure The PINGACCESS for Azure ad* 中的指示，以在 Ping 身分識別網站上使用 Microsoft Azure ad 應用程式 Proxy 來保護髮布的應用程式，並下載最新版本的 PingAccess。

**設定錯誤的應用程式 (AADSTS650056) 錯誤**

1. 確定您從應用程式擁有者所提供的登入位址存取應用程式。 否則，請以其正常處理方式登入應用程式。 在大多數情況下，這會自然自動解決。 如果不是，則此文章可協助疑難排解及解決問題。
2. **如果您的組織擁有應用程式** (表示應用程式註冊是在您的組織中) ：
    - 至少，我們建議您 `User.Read` `openid` 加入來自 **Microsoft Graph** 的或委派許可權。
    - 確定應用程式及其擁有權力都有權。 您可以查看 **API 許可權** 內應用程式註冊的 [**狀態**] 欄，以進行驗證。
    - 在某些情況下，應用程式可能是協力廠商，但是它可能會在您的組織中註冊。 確認此應用程式是否列在應用程式註冊中 (不是企業應用程式) 。
    - 如果您繼續看到此錯誤訊息。 然後，您可能需要建立 **步驟 4** 中所述的同意 URL。
3. **如果您的組織不是應用程式擁有者，且使用它做為協力廠商應用程式**：
    - 如果您是全球/公司系統管理員，您應該會看到同意畫面。 請確認您已勾選「 **代表您的組織同意**」核取方塊。
    - 如果您沒有看到 [同意] 畫面，請刪除企業應用程式，然後再試一次。
    - 如果您繼續看到此錯誤訊息。 然後，您可能需要建立 **步驟 4** 中所述的同意 URL。
4. **手動建立要使用的同意 URL**：如果應用程式是設計用來存取特定資源的，您可能無法使用 Azure 入口網站的同意按鈕，您必須手動產生您的同意 url，並使用此 url。
    - 您將需要 `{App-Id}` `{App-Uri-Id}` 從應用程式擁有者取得及。 `{Tenant-Id}` 將會是您的租使用者識別碼。 這將是 `yourdomain.onmicrosoft.com` 或您的目錄識別碼。
    - 如果應用程式是為資源自行存取，則 `{App-Id}` 和 `{App-Uri-Id}` 將會相同。
5. 如需詳細資訊，請參閱登 [入至 SAML-based 單一登入已設定的應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)時的問題。

**自訂應用程式**

- [將署名新增至您組織的 Azure Active directory 登入頁面](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) -使用您組織的標誌和自訂色彩配置，為您的 Azure active Directory (azure AD) 登入頁面提供一致的外觀與風格。
- [使用 Azure Active Directory 入口網站新增您的自訂功能變數名稱](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) ，每個新 Azure AD 租使用者都附帶一個初始功能變數名稱。 您無法變更或刪除初始功能變數名稱，但是可以新增您組織的名稱。 新增自訂功能變數名稱可協助您建立使用者所熟悉的使用者名稱。
