---
title: 取得 Enterprise 應用程式的清單
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
- "9004342"
- "9837"
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116719"
---
# <a name="get-a-list-of-enterprise-applications"></a>取得 Enterprise 應用程式的清單

1. 若要 **取得企業應用程式** (所有應用程式的清單，或透過 [顯示名稱]、[識別碼]、[識別碼] URIs 等進行篩選 ) 透過 Powershell 命令，請參閱 [AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)。
2. 若要取得服務主體物件的清單， (所有物件或依識別碼篩選) 透過 Powershell 命令，請參閱 [AzureADServicePrincipal (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)。
3. 如果您想要 **取得 SAML 已設定應用程式的清單，下列 PowerShell 腳本** 可能會協助您：

    每個應用程式都是 OAuth 的應用程式或 SAML 應用程式 (庫和非圖庫應用程式) 都會在進行註冊時，在 AAD 中建立兩個物件。 一個稱為 Application 物件，另一個是服務主體物件。 當您使用 PowerShell 來轉儲服務主體物件的屬性時，會發現每個應用程式都有特定數目的標記與其相關聯，例如：

    - OAuth 應用程式會有一個名為 "**WindowsAzureActiveDirectoryIntegratedApp**" 的標記
    - 圖庫 SAML 應用程式會有一個名為 "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" 的標記
    - 非圖庫 SAML 應用程式會有一個名為 "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**" 的標記

    因此，您可以使用這些標記，並找出它所用的應用程式類型。 標記 "**WindowsAzureActiveDirectoryIntegratedApp**" 對所有類型的應用程式是通用的。 您可以使用下列程式碼片段，列出圖庫和非圖庫)  (的所有 SAML 應用程式：

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    如需詳細資訊，請參閱 [在 AZURE AD 中識別具有 SAML 功能的應用程式](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)。

4. **只尋找並列出 Web 應用程式**：使用下列命令來取得應用程式類型為 "Web APP/API" 的所有 Azure AD 應用程式

    Get-AzureADApplication-All： $true |Where-Object {$ _。PublicClient-ne $true} |英尺
5. **單獨尋找並列出原生應用程式**：執行下列命令，以取得所有本機用戶端 (桌面/行動裝置) 應用程式。

    Get-AzureADApplication-All： $true |Where-Object {$ _。PublicClient-eq $true} |英尺
6. **將所有已註冊 AZURE Ad 應用程式的詳細資料匯出至 csv**：下列命令會將所有 azure Ad 應用程式與必要的詳細資料匯出至 csv 檔案：

    - Get-AzureADApplication-All： $true |Select-Object DisplayName、AppID、PublicClient、AvailableToOtherTenants、HomePage、LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" NoTypeInformation 編碼 UTF8

7. **需要匯出未使用之 Azure 應用程式的清單** -審核報告

    只要您有 Azure AD Premium 授權，Azure AD 便可顯示最多30天的應用程式記錄。
    您有兩個選項可保留超過30天的資料。 您可以使用 [AZURE AD 報告 APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 以程式設計方式取得資料，並將其儲存在資料庫中。 或者，您可以將審核記錄檔整合到協力廠商 SIEM 系統。

    您也可以在 Azure Active directory>應用程式註冊>下載>所有應用程式/擁有的應用程式中，下載所有應用程式和擁有應用程式的應用程式清單。

    若要透過 MS Graph 取得應用程式的清單，請參閱[list application-microsoft Graph 1.0](https://docs.microsoft.com/graph/api/application-list)及[application resource type-microsoft Graph 1.0](https://docs.microsoft.com/graph/api/resources/application)。
