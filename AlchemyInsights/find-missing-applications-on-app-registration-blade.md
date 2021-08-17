---
title: 尋找應用程式註冊 blade 上遺失的應用程式
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
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057093"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>尋找應用程式註冊 blade 上遺失的應用程式

1. 在應用程式註冊入口網站上找不到應用程式。

    如果應用程式是多租使用者應用程式，且已在其他租使用者中註冊，它將不會顯示在 [應用程式註冊 blade] 底下。 不過，您可能會在 Enterprise 應用程式的刀片式伺服器之後找到它 (之後，才會將其存取之後，) 且已在您的租使用者中建立服務主體。 如需詳細資訊，請參閱[在 Azure AD 中 & 服務主體-Microsoft 身分識別平臺中的應用程式](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。
2. 即使您是系統管理員，還是無法在應用程式註冊 blade 中查看應用程式。

    請確認您位於 Azure 入口網站上的正確目錄。
3. 我的應用程式並未列在 Enterprise 應用程式邊欄下，但是當我查詢 PowerShell 命令時，它會顯示。

    有時候，在您從 Azure 入口網站刪除應用程式後，該應用程式不會顯示在入口網站中，但可能尚未完全刪除。 如需詳細資訊，請參閱：
    - 您可以取得先前刪除之應用程式的清單，並查看應用程式是否會顯示在清單中（使用 Powershell 命令： **AzureADDeletedApplication）**。 若要深入瞭解，請參閱 [AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)。
    - 如果您想要完全移除應用程式，您可以在 PowerShell: **remove-ObjectId** 中嘗試下列各項。 若要深入瞭解，請參閱 [ (AzureAD) 中的 Remove-AzureADApplication ](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)。
    - 或者，您也可以嘗試使用下列 Powershell 命令還原已刪除的應用程式： **Restore AzureADDeletedApplication-ObjectId**。 若要深入瞭解，請參閱 [Restore-AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)。
4. 在我的新 Azure 租使用者中找不到所有預先安裝的企業應用程式清單。

    根據預設，Azure AD 中沒有預先安裝的企業應用程式。 您必須從 Azure AD 圖庫或新增非圖庫應用程式中，以手動方式從 ' 新增應用程式」選項中新增它。 若要深入瞭解，請參閱[快速入門：將應用程式新增至您的 Azure Active Directory (Azure AD) 租使用者](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)。
    如果您是全域系統管理員，則可以使用[Microsoft 365 App Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)輕鬆存取您的應用程式。
5. 找不到我的應用程式入口網站上的應用程式。

    確定應用程式未隱藏于 [我的應用程式集合] 頁面。 若要深入瞭解，請參閱 [我的應用程式入口網站-AZURE AD 中的集合 (預覽) ](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)。
6. 若要從 [我的應用程式入口網站] 啟動應用程式，請參閱 [尋找 & 在我的應用程式入口網站-AZURE AD 上使用 app](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)。
7. Office 365在安裝之後，移動器應用程式不會顯示在 Enterprise 應用程式邊欄中。

    「Office 365 移動器」應用程式是一種多租戶應用程式，不需要使用 Enterprise 應用程式註冊的「圖庫應用程式」區段新增至 AAD。 若要存取 Office 365 移動器應用程式，只要登入 app，就會要求使用者同意許可權。 一旦使用者提供同意，此應用程式會自動以您已登入的電子郵件識別碼加入租使用者。

    登入至應用程式之後，您應該可以在 AAD 中的 Enterprise 應用程式」刀片式伺服器底下找到此應用程式的專案。 您必須輸入完整的名稱（即 "Office 365 移動器" 或直接搜尋 "Office"），才可搜尋該應用程式，並且應該列出該應用程式。 若要深入瞭解，請參閱[Office 365 移動器說它已經安裝，但並未列于 Enterprise 應用程式庫中](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)。
8. [快速入門：查看使用 Azure Active Directory (Azure ad) 租使用者的應用程式清單。身分識別管理](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal)說明如何查看已設定為使用 azure ad 租使用者作為身分識別提供者的應用程式（也稱為應用程式）， (IdP) 。
9. [疑難排解常見問題新增或移除 Azure Active Directory 的應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps)可協助您瞭解人們在 Azure Active Directory 中查看應用程式的常見問題。
