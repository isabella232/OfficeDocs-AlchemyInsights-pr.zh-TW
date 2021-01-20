---
title: 疑難排解使用者問題
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886802"
---
# <a name="announcements"></a>公告

依照 Google 有關測試相容性的指引，測試您的應用程式是否受到影響。 可在 https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support取得 Google 的指引。

請確認您在使用家庭用戶 Google 帳戶登入使用者時，使用系統網頁檢視或系統瀏覽器。 如需詳細資訊，請參閱 [僅使用 Chrome 瀏覽器登入應用程式問題](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)。


**我無法在我的 Azure Active Directory 中建立新使用者**

若要針對無法在 Azure Active Directory 中建立新使用者的問題進行疑難排解，請執行下列步驟：

1. 請確保您已獲授權建立新的標準使用者。 只有 Azure Active Directory (AD) 中的全域系統管理員或使用者系統管理員角色可以建立新的標準使用者。 如果您不是上述其中一種角色，請要求系統管理員將您新增為這些角色之一或為您建立新的使用者帳戶。
2. 請確保使用者名稱所在的網域是在您的 Azure AD 得到驗證。 如果您的 Azure AD 中沒有任何已驗證的自訂網域名稱，您可以使用您的 Azure AD 初始網域，結尾是 *. onmicrosoft.com。
3. 請確保使用者名稱所在的網域並非是從內部部署 AD 同盟的 Azure AD。 無法將使用者新增至具有從內部部屬同盟的網域名稱雲端中。
4. 請確保其他使用者或聯絡人不具有您要指派給新使用者的使用者名稱。 使用者名稱在 Azure Active Directory 中必須是唯一的。
5. 請參閱 Azure Active Directory 的 [Azure Active Directory 角色和系統管理員](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators)。
6. 請參閱 Azure Active Directory 的 [網域名稱](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains)。
7. 請檢視 [稽核記錄檔](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) 以查看更多關於最近建立或刪除的使用者的詳細資訊，例如誰執行該動作，以及何時執行。
8. 如需有關新增使用者的詳細資訊，請參閱 [使用 [Microsoft Azure 入口網站] 以在 Azure AD 中建立新使用者](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) 。
9. 如需有關 Azure Active Directory 中的系統管理員角色許可權詳細資訊，請參閱 [Azure Active Directory 系統管理角色](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)。
10. 如需有關使用 Azure AD Powershell 建立使用者的詳細資訊，請參閱 [使用 Azure AD PowerShell 建立新使用者](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser)。

**自助註冊的問題**

若要疑難排解有關自助註冊的問題，請執行下列步驟：

1. 若要使用您的應用程式進行自助註冊，請先為您的租用戶啟用自助註冊。 
2. 若要讓應用程式支援自助註冊，請將它新增到您的使用者流程。 下次您移至該應用程式的登入頁面時，您會看到選項 **_沒有帳戶嗎？建立一個！_* _。 這會啟動自助註冊程式。
3. 如需有關如何使用自助註冊以填入 Azure Active Directory 中的組織詳細資訊，請參閱 [Azure Active Directory 的自助註冊](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup)。
4. 當您將使用者流程與一個或多個應用程式建立關聯之後，造訪該應用程式的使用者將可以使用使用者流程中設定的選項，註冊並取得來賓帳戶。 如需有關註冊並取得來賓帳戶的詳細資訊，使用者可以查看 [來賓使用者的自助註冊](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow)。

_ *邀請外部使用者的問題**

若要針對邀請外部使用者的問題進行疑難排解，請執行下列步驟：

請確保您寄邀請給使用者的電子郵件地址與使用者用於登入的電子郵件地址相同。 如果您將此邀請傳送到使用者的 proxy 電子郵件地址，則該使用者會無法兌換。 如需詳細資訊，請參閱 [Azure Active Directory B2B 文件](https://docs.microsoft.com/azure/active-directory/external-identities/)。

**我無法指派授權給使用者**

若要疑難排解有關指派授權給使用者的問題，請執行下列步驟：

1. 若要管理使用者授權，請確定您使用的帳戶屬於下列必要系統管理員角色的其中一個：全域系統管理員、授權系統管理員或使用者系統管理員。 您可以在使用者刀鋒視窗的 **目錄角色** 索引標籤中查看使用者的角色。
2. 如果您正在使用 Azure 入口網站，且無法指派授權，請按一下右上角的通知。 這會開啟一個具有何處發生錯誤詳細資料的刀鋒視窗。 在大部分的情況下，您可以瞭解並解決問題。
3. 將授權指派給使用者之前，請先確定已為使用者設定 **使用位置** 屬性。 藉由在使用者刀鋒視窗上檢視 **設定檔** 索引標籤，驗證使用者是否已設定該屬性。
4. 請確定您要指派的產品已具備足夠的可用授權。 您可以在 [Microsoft Azure 入口網站] 中查看可用的授權數，可在 [Azure Active Directory-> 授權-> 所有產品](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products)。
5. 使用者可能已經有另一種授權，其服務與您嘗試指派的新授權相衝突。 例如，如果使用者已啟用 Exchange Online (方案 1) 服務，您將無法使用 Exchange Online (方案 2) 指派授權。 停用其中一個服務以允許新的授權指派。 如果您正在使用的 [Microsoft Azure 入口網站] 或 PowerShell Cmdlet，**問題詳細資料** 頁面會列出造成衝突的特定服務。
6. 如果您嘗試移除授權且移除失敗，使用者可能會使用其他服務的授權，而這些服務則會根據您嘗試想移除的服務而定。 如果您正在使用 [Microsoft Azure 入口網站] 或 PowerShell Cmdlet，則錯誤訊息將會列出具有依賴性的特定服務。
7. 如果您想瞭解為什麼要由使用者新增或移除授權 (例如，貴組織中的其他人員可能已進行變更)，請查看稽核紀錄檔。 將篩選設定為 **授權活動** 以顯示所有的修改，包括執行它們的「執行者」。
8. 如果您正在使用 Exchange Online，您租用戶中的部分使用者可能會使用相同的 proxy 位址值進行錯誤設定。 在這種情況下，授權作業失敗時，您可能會看到一般錯誤訊息。 [本文](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) 包含此問題的詳細資訊，包括有關 [如何使用遠端 PowerShell 連線到 Exchange Online](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell) 的資訊。若要識別您租用戶的哪些使用者，包含相同的 proxy 位址，請執行此 Exchange Online Cmdlet：

執行

Get-Recipient | where {$_.EmailAddresses -match <user principal name>} | fL Name, RecipientType,emailaddresses





