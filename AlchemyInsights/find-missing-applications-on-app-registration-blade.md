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
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123046"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>尋找應用程式註冊 blade 上遺失的應用程式

1. 在應用程式註冊入口網站上找不到應用程式。

    如果應用程式是多租使用者應用程式，且已在其他租使用者中註冊，它將不會顯示在 [應用程式註冊 blade] 底下。 不過，您可能會在已存取企業應用程式時，將其放在「企業應用程式 blade」底下 (後) ，且已在您的租使用者中建立服務主體。 如需詳細資訊，請參閱 [AZURE AD-Microsoft identity platform 中的應用程式 & 服務主體](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)。
2. 即使您是系統管理員，還是無法在應用程式註冊 blade 中查看應用程式。

    請確認您位於 Azure 入口網站上的正確目錄。
3. 我的應用程式未列在 [企業應用程式] 邊欄底下，但是它會在查詢 PowerShell 命令時顯示。

    有時候，在您從 Azure 入口網站刪除應用程式後，該應用程式不會顯示在入口網站中，但可能尚未完全刪除。 如需詳細資訊，請參閱：
    - 您可以取得先前刪除之應用程式的清單，並查看應用程式是否會顯示在清單中（使用 Powershell 命令： **AzureADDeletedApplication）**。 若要深入瞭解，請參閱 [AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)。
    - 如果您想要完全移除應用程式，您可以在 PowerShell: **remove-ObjectId** 中嘗試下列各項。 若要深入瞭解，請參閱 [ (AzureAD) 中的 Remove-AzureADApplication ](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)。
    - 或者，您也可以嘗試使用下列 Powershell 命令還原已刪除的應用程式： **Restore AzureADDeletedApplication-ObjectId**。 若要深入瞭解，請參閱 [Restore-AzureADDeletedApplication (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)。
4. 在我的新 Azure 租使用者中找不到所有預先安裝的企業應用程式清單。

    根據預設，Azure AD 中沒有預先安裝的企業應用程式。 您必須從 Azure AD 圖庫或新增非圖庫應用程式中，以手動方式從 ' 新增應用程式」選項中新增它。 若要深入瞭解，請參閱 [快速入門：將應用程式新增至您的 Azure Active Directory 中 (AZURE AD) 租使用者](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)。
    如果您是全域系統管理員，您可以使用 [Microsoft 365 應用程式啟動器](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)輕鬆存取您的應用程式。
5. 找不到我的應用程式入口網站上的應用程式。

    確定應用程式未隱藏于 [我的應用程式集合] 頁面。 若要深入瞭解，請參閱 [我的應用程式入口網站-AZURE AD 中的集合 (預覽) ](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections)。
6. 若要從 [我的應用程式入口網站] 啟動應用程式，請參閱 [尋找 & 在我的應用程式入口網站-AZURE AD 上使用 app](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access)。
7. 安裝後，Office 365 移動器應用程式不會顯示在企業應用程式邊欄上。

    「Office 365 移動器」應用程式是一種多租戶應用程式，不需要使用 [企業應用程式註冊] 底下的「圖庫應用程式」區段新增至 AAD。 若要存取 Office 365 移動器應用程式，只要登入 app，就會要求使用者同意許可權。 一旦使用者提供同意，此應用程式會自動以您已登入的電子郵件識別碼加入租使用者。

    登入至應用程式之後，您應該可以在 AAD 中的企業應用程式的刀片式伺服器底下找到此應用程式的專案。 若要搜尋該應用程式，請輸入完整名稱，例如 "Office 365 移動器" 或直接搜尋 "Office"，並且應該列出該應用程式。 若要深入瞭解，請參閱 [Office 365 移動器說它已經安裝，但並未列在企業應用程式圖庫中](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)。
8. [快速入門：查看使用您的 Azure Active Directory (AZURE ad) 租使用者的應用程式清單。身分識別管理](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) 顯示如何查看已設定為使用 azure AD 租使用者作為身分識別提供者的應用程式（也稱為應用程式）， (IdP) 。
9. [疑難排解常見問題新增或移除應用程式至 Azure Active directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) 可協助您瞭解人們在 Azure active directory 中查看應用程式的常見問題。
