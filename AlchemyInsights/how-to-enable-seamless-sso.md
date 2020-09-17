---
title: 如何啟用無縫 SSO
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780518"
---
# <a name="how-to-enable-seamless-sso"></a>如何啟用無縫 SSO

透過 [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)啟用無縫 SSO。
  
如果您是執行 Azure AD Connect 的全新安裝，請選擇 [自訂安裝路徑](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)。 在 [ **使用者登入** ] 頁面上，選擇 [ **啟用單一登入** ] 選項。
  
若要確認您已正確啟用無縫 SSO，請執行下列動作：
  
1. 以全域系統管理員身分登入 [Azure Active Directory 系統管理中心](https://aad.portal.azure.com) 。

2. 在左窗格中選取 [ **Azure Active Directory** ]。

3. 確認 **已啟用**無縫單一登入。

若要深入瞭解，請參閱 [Azure Active Directory 無縫單一 Sign-On：快速入門](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。
  