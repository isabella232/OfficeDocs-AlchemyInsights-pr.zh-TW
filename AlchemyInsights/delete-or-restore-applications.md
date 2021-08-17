---
title: 刪除或還原應用程式
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102562"
---
# <a name="delete-or-restore-applications"></a>刪除或還原應用程式

**若要從您的 AZURE AD 租使用者刪除應用程式**：

1. 在 **Azure AD 入口網站** 中，選取 [ **Enterprise 應用程式**]。 然後尋找並選取您要刪除的應用程式。
2. 在左窗格的 [ **管理** ] 區段中，選取 [ **屬性**]。
3. 選取 [ **刪除**]，然後選取 **[是]** 以確認您要從 Azure AD 租使用者刪除應用程式。

如需如何刪除應用程式的詳細資訊，請參閱[快速入門：從您的 Azure Active Directory (Azure AD) 租使用者刪除應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)。

在 PowerShell 中， [AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) Cmdlet 會從 Azure Active Directory 中的特定應用程式移除應用程式 Proxy 設定，而且可以完全刪除應用程式（若有指定）。

您可以使用 PowerShell **還原已刪除的應用程式** 。 在您想要還原的應用程式被識別後，您可以使用 [AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)還原它。
