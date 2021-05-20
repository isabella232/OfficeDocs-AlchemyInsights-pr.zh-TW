---
title: 建立使用者
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569702"
---
# <a name="create-user"></a>建立使用者

**公告：**

- [從 Google 開始，在2021年1月4日開始的 Web 視圖登入支援已過時](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) 。 測試您的應用程式是否會受到 Google 對測試相容性 [的指導](https://go.microsoft.com/fwlink/?linkid=2157323) 所影響。
- 使用使用者 Google 帳戶登入時，請確定您使用系統 web 視圖或系統瀏覽器。 如需詳細資訊，請參閱 [僅使用 Chrome 瀏覽器登入應用程式問題](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。

**我無法在我的 Azure Active Directory 中建立新使用者**

1. 請確保您已獲授權建立新的標準使用者。 Azure Active Directory (AD) 中只有全域系統管理員或使用者系統管理員角色可以建立新的標準使用者。 如果您不是上述其中一種角色，請要求系統管理員將您新增為這些角色之一或為您建立新的使用者帳戶。
1. 請確保使用者名稱所在的網域是在您的 Azure AD 得到驗證。 如果您的 Azure AD 中沒有任何已驗證的自訂網域名稱，您可以使用您的 Azure AD 初始網域，結尾是 *. onmicrosoft.com。
1. 請確保使用者名稱所在的網域並非是從內部部署 AD 同盟的 Azure AD。 無法將使用者新增至具有從內部部屬同盟的網域名稱雲端中。
1. 請確保其他使用者或聯絡人不具有您要指派給新使用者的使用者名稱。 使用者名稱在 Azure Active Directory 中必須是唯一的。
1. 請參閱 Azure Active Directory 的 [Azure Active Directory 角色和系統管理員](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 請參閱 Azure Active Directory 的 [網域名稱](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
1. 請檢視 [稽核記錄檔](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) 以查看更多關於最近建立或刪除的使用者的詳細資訊，例如誰執行該動作，以及何時執行。
1. 如需新增使用者的詳細資訊，請參閱 [使用 azure 入口網站在 AZURE AD 中建立新的使用者](/azure/active-directory/active-directory-users-create-azure-portal)。
1. [AZURE AD 系統管理角色](/azure/active-directory/active-directory-assign-admin-roles)： Azure Active Directory 中的系統管理員角色許可權
1. 您也可以 [使用 AZURE AD PowerShell 來建立新的使用者](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)。
