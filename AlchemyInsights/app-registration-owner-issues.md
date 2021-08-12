---
title: 應用程式註冊擁有人問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951124"
---
# <a name="app-registration-owner-issues"></a>應用程式註冊擁有人問題

以下是可將主體新增為應用程式註冊負責人的可用方法：

- 使用 Azure AD PowerShell 模組-

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    參考： [載入 AzureADApplicationOwner (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- 使用 Azure CLI- `az ad app owner add`

    參照： [az ad 應用程式擁有](https://docs.microsoft.com/cli/azure/ad/app/owner)者
- 使用 MS Graph-

    參考：[新增擁有者-Microsoft Graph v 1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- 使用 Azure AD 入口網站-流覽至 [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > 應用程式註冊 > 選取應用程式 > 擁有者 > 新增擁有者

**即使您是該應用程式的擁有者，也無法在應用程式註冊 blade 上查看您的應用程式？**

應用程式的擁有者不是系統管理角色。 如果已啟用設定 [ [限制存取 AZURE AD 管理入口網站](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) ]，則只有系統管理員可以在應用程式註冊入口網站上查看應用程式。 若要讓擁有者能夠查看應用程式，請停用此設定 (將此設定設為 [) 否]，或將系統管理員角色指派給擁有者，只指定特定的應用程式。 不過，您會需要 Azure AD Premium P2 授權並啟用[Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)。
