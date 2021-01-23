---
title: 無縫 SSO 使用者登入問題
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
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/21/2021
ms.locfileid: "49919198"
---
# <a name="seamless-sso-user-sign-in-issues"></a>無縫 SSO 使用者登入問題

使用者驗證之後，瀏覽器將會快取使用者的認證，因此，在相同的瀏覽器上，應用程式會自動以相同的帳戶登入。 這可能會使另一位使用者或單一使用者在一個裝置上登入多個帳戶變得很困難。 若要解決此事項：1。 嘗試在另一個瀏覽器登入。 2. 請清除瀏覽器的快取和/或 cookie，然後再次嘗試登入。

如果您仍遇到登入問題，建議您先執行下列步驟，以診斷及自動化解決步驟：

1. 安裝 [My Apps Secure Browser Extension](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) ，以協助 Azure Active Directory (azure AD) ，以在使用 Azure 入口網站中的測試體驗時，提供更好的診斷和解決方法。
2. 使用 Azure 入口網站中 app configuration 頁面上的測試體驗，再現錯誤。 若要深入瞭解，請參閱 [調試 SAML-based 單一登入應用程式](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues)。
3. 如果您在 Azure 入口網站中使用 My Apps Secure Browser Extension 的測試體驗，您可以 **略過步驟 4**。
4. 若要開啟 [SAML-based 單一登入設定] 頁面：
    - 開啟 [Azure 入口網站](https://portal.azure.com/) ，並以 **全域系統管理員** 或 **Coadmin** 登入。
    - 選取主要左導覽功能表頂端的 [**所有服務**]，以開啟 **Azure Active Directory 擴充**。
    - 在 [篩選搜尋] 方塊中，輸入 "Azure Active Directory"，然後選取 **Azure Active directory** 專案。
    - 從 Azure Active Directory 左手手流覽功能表中選取 [ **企業應用程式** ]。
    - 選取 [ **所有應用程式** ]，以查看所有應用程式的清單。 如果您沒有看到您想要顯示的應用程式，請使用 [**所有應用程式] 清單** 頂端的 [**篩選**] 控制項，並將 [**顯示**] 選項設定為 [**所有應用程式**]。
    - 選取您要設定單一登入的應用程式。
    - 在應用程式載入之後，從應用程式的左手流覽功能表中選取 [ **單一登入** ]。
    - 選取 [ **SAML-BASED SSO**]。
5. 根據錯誤，若要深入瞭解建議遵循的步驟，請參閱登 [入 SAML-based 單一登入已設定之應用程式的問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory)。
6. 若要疑難排解其他使用者簽署問題，請參閱下列指導：
    - [單一 Sign-On SAML 通訊協定](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [操作方法：使用 Azure Active Directory 報告疑難排解簽入錯誤](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [未預期的同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [使用者同意錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [從我的應用程式登入時發生問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Application 登入頁面上的錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [登入 Microsoft 應用程式時的問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
