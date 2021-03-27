---
title: 取得企業應用程式的清單
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
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379802"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="cd657-102">取得企業應用程式的清單</span><span class="sxs-lookup"><span data-stu-id="cd657-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="cd657-103">若要 **取得企業應用程式** (所有應用程式的清單，或透過 [顯示名稱]、[識別碼]、[識別碼] URIs 等進行篩選 ) 透過 Powershell 命令，請參閱 [AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)。</span><span class="sxs-lookup"><span data-stu-id="cd657-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="cd657-104">若要取得服務主體物件的清單， (所有物件或依識別碼篩選) 透過 Powershell 命令，請參閱 [AzureADServicePrincipal (AzureAD) ](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)。</span><span class="sxs-lookup"><span data-stu-id="cd657-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="cd657-105">如果您想要 **取得 SAML 已設定應用程式的清單，下列 PowerShell 腳本** 可能會協助您：</span><span class="sxs-lookup"><span data-stu-id="cd657-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="cd657-106">每個應用程式都是 OAuth 的應用程式或 SAML 應用程式 (庫和非圖庫應用程式) 都會在進行註冊時，在 AAD 中建立兩個物件。</span><span class="sxs-lookup"><span data-stu-id="cd657-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="cd657-107">一個稱為 Application 物件，另一個是服務主體物件。</span><span class="sxs-lookup"><span data-stu-id="cd657-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="cd657-108">當您使用 PowerShell 來轉儲服務主體物件的屬性時，會發現每個應用程式都有特定數目的標記與其相關聯，例如：</span><span class="sxs-lookup"><span data-stu-id="cd657-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="cd657-109">OAuth 應用程式會有一個名為 "**WindowsAzureActiveDirectoryIntegratedApp**" 的標記</span><span class="sxs-lookup"><span data-stu-id="cd657-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="cd657-110">圖庫 SAML 應用程式會有一個名為 "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**" 的標記</span><span class="sxs-lookup"><span data-stu-id="cd657-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="cd657-111">非圖庫 SAML 應用程式會有一個名為 "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**" 的標記</span><span class="sxs-lookup"><span data-stu-id="cd657-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="cd657-112">因此，您可以使用這些標記，並找出它所用的應用程式類型。</span><span class="sxs-lookup"><span data-stu-id="cd657-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="cd657-113">標記 "**WindowsAzureActiveDirectoryIntegratedApp**" 對所有類型的應用程式是通用的。</span><span class="sxs-lookup"><span data-stu-id="cd657-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="cd657-114">您可以使用下列程式碼片段，列出圖庫和非圖庫)  (的所有 SAML 應用程式：</span><span class="sxs-lookup"><span data-stu-id="cd657-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="cd657-115">如需詳細資訊，請參閱 [在 AZURE AD 中識別具有 SAML 功能的應用程式](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)。</span><span class="sxs-lookup"><span data-stu-id="cd657-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="cd657-116">**只尋找並列出 Web 應用程式**：使用下列命令來取得應用程式類型為 "Web APP/API" 的所有 Azure AD 應用程式</span><span class="sxs-lookup"><span data-stu-id="cd657-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="cd657-117">Get-AzureADApplication-All： $true |Where-Object {$ _。PublicClient-ne $true} |英尺</span><span class="sxs-lookup"><span data-stu-id="cd657-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="cd657-118">**單獨尋找並列出原生應用程式**：執行下列命令，以取得所有本機用戶端 (桌面/行動裝置) 應用程式。</span><span class="sxs-lookup"><span data-stu-id="cd657-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="cd657-119">Get-AzureADApplication-All： $true |Where-Object {$ _。PublicClient-eq $true} |英尺</span><span class="sxs-lookup"><span data-stu-id="cd657-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="cd657-120">**將所有已註冊 AZURE Ad 應用程式的詳細資料匯出至 csv**：下列命令會將所有 azure Ad 應用程式與必要的詳細資料匯出至 csv 檔案：</span><span class="sxs-lookup"><span data-stu-id="cd657-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="cd657-121">Get-AzureADApplication-All： $true |Select-Object DisplayName、AppID、PublicClient、AvailableToOtherTenants、HomePage、LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="cd657-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="cd657-122">Export-Csv "C:\AzureADApps.csv" NoTypeInformation 編碼 UTF8</span><span class="sxs-lookup"><span data-stu-id="cd657-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="cd657-123">**需要匯出未使用之 Azure 應用程式的清單** -審核報告</span><span class="sxs-lookup"><span data-stu-id="cd657-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="cd657-124">只要您擁有 Azure AD Premium 授權，Azure AD 便可顯示最多30天的應用程式記錄。</span><span class="sxs-lookup"><span data-stu-id="cd657-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="cd657-125">您有兩個選項可保留超過30天的資料。</span><span class="sxs-lookup"><span data-stu-id="cd657-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="cd657-126">您可以使用 [AZURE AD 報告 APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) 以程式設計方式取得資料，並將其儲存在資料庫中。</span><span class="sxs-lookup"><span data-stu-id="cd657-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="cd657-127">或者，您可以將審核記錄檔整合到協力廠商 SIEM 系統。</span><span class="sxs-lookup"><span data-stu-id="cd657-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="cd657-128">您也可以在 Azure Active directory>應用程式註冊>下載>所有應用程式/擁有的應用程式中，下載所有應用程式和擁有應用程式的應用程式清單。</span><span class="sxs-lookup"><span data-stu-id="cd657-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="cd657-129">若要透過 MS Graph 取得應用程式的清單，請參閱 [list application-Microsoft graph 1.0](https://docs.microsoft.com/graph/api/application-list) 及 [application Resource Type-Microsoft graph 1.0 1.0](https://docs.microsoft.com/graph/api/resources/application)。</span><span class="sxs-lookup"><span data-stu-id="cd657-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
