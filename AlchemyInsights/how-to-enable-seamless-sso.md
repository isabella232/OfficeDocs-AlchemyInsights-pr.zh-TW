---
title: 如何啟用無縫 SSO
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 565ec53a3d9f8863562ac828e21a4a153c61ae88
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825722"
---
# <a name="how-to-enable-seamless-sso"></a>如何啟用無縫 SSO

透過 [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect)啟用無縫 SSO。
  
如果您是執行 Azure AD Connect 的全新安裝，請選擇 [自訂安裝路徑](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom)。 在 [ **使用者登入** ] 頁面上，選擇 [ **啟用單一登入** ] 選項。
  
若要確認您已正確啟用無縫 SSO，請執行下列動作：
  
1. 以全域系統管理員身分登入 [Azure Active Directory 系統管理中心](https://aad.portal.azure.com) 。

2. 在左側窗格中，選取 **[Azure Active Directory]**。

3. 確認 **已啟用** 無縫單一登入。

若要深入瞭解，請參閱 [Azure Active Directory 無縫單一 Sign-On：快速入門](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start)。
  