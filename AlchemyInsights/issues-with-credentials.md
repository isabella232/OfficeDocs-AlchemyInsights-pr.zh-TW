---
title: 認證的問題
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
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052944"
---
# <a name="issues-with-credentials"></a>認證的問題

[Microsoft identity platform 和 OAuth 2.0 用戶端認證流程](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 說明如何直接針對 OAuth 2.0 用戶端認證授與流程進行程式設計。

**如何管理應用程式的密碼或憑證認證？**

在 Azure CLI 中，您可以使用 [az ad app 認證](https://docs.microsoft.com/cli/azure/ad/app/credential) 來刪除、列出或重設應用程式的密碼或憑證認證。

**我的使用者如何重設密碼？**

使用者必須先 [註冊自助密碼重設，](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) 才能重設密碼。 使用者註冊後，可依照本文中的指示重設密碼： [重設您的工作或學校密碼](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)。

**我的使用者如何變更密碼？**

使用者可以遵循本文中的步驟變更其密碼： [如何變更您的密碼](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)。
他們也可以 [管理兩步驟驗證的應用程式密碼](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)。

**我的使用者在變更或重設其密碼時收到錯誤**

此連結會提供使用者嘗試重設密碼時可能發生的常見問題資訊： [一般問題及其解決方案](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)

**重設使用者密碼時出現問題**

- 請確定您有權重設密碼。 *只有全域、密碼和使用者管理員才能重設使用者密碼。* 全域管理員也可以重設其他特權管理員的密碼。

- 請確定您瞭解授權需求：

  - 您的組織中至少必須已指派一個授權：
    - **僅限雲端使用者** -任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic
    - **雲端和/或內部部署使用者** -Azure AD Premium P1 或 P2、Enterprise 可移動性 + SECURITY (EMS) 或安全生產力 (SPE) 
    - 若要深入瞭解授權需求，請參閱 [AZURE AD 自助密碼重設的授權需求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)。
- 若要重設使用者的密碼，請在 Azure AD 中尋找使用者。 然後，在該使用者的 [一覽] 邊欄上，按一下 [重設密碼] 按鈕。

**[密碼重設] 按鈕會灰顯**

您未獲授權，無法重設 **此** 使用者的密碼。 *只有全域、密碼和使用者管理員才能重設使用者密碼。* 全域管理員也可以重設其他特權管理員的密碼。

**我沒有看到密碼重設的刀片式伺服器**

您未獲授權，無法重設密碼。 *只有全域、密碼和使用者管理員才能重設使用者密碼。* 全域管理員也可以重設其他特權管理員的密碼。

**在密碼重設中看不到內部部署整合刀片式伺服器**

- 內部部署整合刀片式伺服器只會出現在混合環境中，也就是說，您使用密碼寫回來處理內部部署使用者的密碼。

- 在下列情況中看不到此邊欄：

  - 您不是使用密碼回寫
  - 密碼寫回的安裝/連線發生問題
  - Azure AD Connect 的安裝/連線發生問題
  - 如需有關密碼寫回問題的疑難排解步驟，請參閱 [密碼寫回疑難排解](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)

**我不知道如何重設使用者的密碼**

1. 以適當的系統管理員身分登入 Azure 入口網站。
2. 移至 [ **使用者和群組** ] 邊欄，選取 [ **所有使用者**]。
3. 從清單中選取使用者。
4. 針對選取的使用者，選取 **[概述**]，然後在命令列中選取 [ **重設密碼**]。
5. 選取 [ **重設密碼** ] 按鈕，然後依照畫面上的指示進行。
    - 僅透過 **Azure 入口網站** 支援密碼回寫進行重設。

**我從 Office 365 Admin 入口網站或 Office 365 行動應用程式重設內部部署使用者的密碼，但使用者仍無法登入**

此入口網站不支援密碼回寫。 在 Azure 入口網站中重新重設使用者的密碼。
