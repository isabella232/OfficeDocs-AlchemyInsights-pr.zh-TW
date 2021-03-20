---
title: 使用者管理問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897774"
---
# <a name="user-management-issues"></a>使用者管理問題

**如果我停用屬性 '需要使用者指派' (將此屬性設定為 No)，目前已指派給應用程式的使用者會發生什麼情況？**

停用 **[需要使用者指派]** 不會影響目前已指派的使用者。 停用此屬性只會允許所有使用者存取應用程式。 所有列出的使用者，以及已指派給應用程式中群組的使用者仍然有效。

- 若要將您的應用程式限制為特定一組使用者，請參閱 - [Azure AD 應用程式限制一組使用者 - Microsoft 身分識別平台 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.) (部分機器翻譯)。
- 若要指派使用者和群組至 Azure Active Directory (Azure AD) 中的企業應用程式 (從 Azure 入口網站內或使用 PowerShell)，請參閱[在 Azure Active Directory 中管理應用程式的使用者指派](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal) (部分機器翻譯)。
- 若要委派應用程式建立和管理權限，請參閱[委派應用程式管理系統管理員權限 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles) (部分機器翻譯)。
- **向使用者隱藏特定企業應用程式** - 使用下列步驟，從 **MyApps** 面板中隱藏所有 Microsoft 365 應用程式。 應用程式仍然顯示在 Office 365 入口網站中。

 1. 以您目錄的全域管理員身分登入 Azure 入口網站。 
 2. 選取 **[Azure Active Directory]**。 
 3. 選取 **[使用者]**。 
 4. 選取 **[使用者設定]**。 
 5. 在 **[企業應用程式]** 下，按一下 **[管理終端使用者如何啟動和檢視其應用程式]**。 
 6. 針對 **[使用者只能在 Office 365 入口網站中查看 Office 365 應用程式]**，請按一下 **[是]**。 
 7. 按一下 **[儲存]**。 
 8. 有關詳細資料，請參閱 [在 Azure AD 中隱藏使用者的企業應用程式之體驗 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.) (部分機器翻譯)

- 如果您提供軟體即服務 (SaaS) 應用程式給許多組織，您可以將應用程式設定為接受來自任何 Azure Active Directory (Azure AD) 租用戶的登入。 此設定稱為「將您的應用程式設為多租用戶」。 任何 Azure AD 租用戶中的使用者，在同意將他們的帳戶用於您的應用程式之後，就可以登入您的應用程式。 有關詳細資訊，請參閱 [建立登入 Azure AD 使用者的應用程式 - Microsoft 身分識別平台 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant) (部分機器翻譯)。

- **終端用者被指派至應用程式後，如何存取應用程式？**

企業應用程式刀鋒視窗中的每個應用程式都有供使用者存取的連結。 使用者也可以透過 **MyApps** 入口網站輕鬆存取應用程式。

- **想知道使用者所使用的應用程式和應用程式類型嗎？**

您可以從 **portal.azure.com > Azure Active Directory> 登入> 下載報告** 下載最近 30 天的登入報告。

- 了解如何[將整個租用戶系統管理員同意授與給應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) (部分機器翻譯) 和[設定使用者同意應用程式的方式](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) (部分機器翻譯)。

- 了解[同意的運作方式](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) (部分機器翻譯) 和[管理應用程式的同意](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests) (部分機器翻譯)。


