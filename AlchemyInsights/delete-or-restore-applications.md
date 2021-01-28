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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013930"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="ab078-102">刪除或還原應用程式</span><span class="sxs-lookup"><span data-stu-id="ab078-102">Delete or restore applications</span></span>

<span data-ttu-id="ab078-103">**若要從您的 AZURE AD 租使用者刪除應用程式**：</span><span class="sxs-lookup"><span data-stu-id="ab078-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="ab078-104">在 **AZURE AD 入口網站** 中，選取 [ **企業應用程式**]。</span><span class="sxs-lookup"><span data-stu-id="ab078-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="ab078-105">然後尋找並選取您要刪除的應用程式。</span><span class="sxs-lookup"><span data-stu-id="ab078-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="ab078-106">在左窗格的 [ **管理** ] 區段中，選取 [ **屬性**]。</span><span class="sxs-lookup"><span data-stu-id="ab078-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="ab078-107">選取 [ **刪除**]，然後選取 **[是]** 以確認您要從 Azure AD 租使用者刪除應用程式。</span><span class="sxs-lookup"><span data-stu-id="ab078-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="ab078-108">如需如何刪除應用程式的詳細資訊，請參閱 [快速入門：從 Azure Active Directory (AZURE AD) 租使用者刪除應用程式](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)。</span><span class="sxs-lookup"><span data-stu-id="ab078-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="ab078-109">在 PowerShell 中， [AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) Cmdlet 會從 Azure Active Directory 中的特定應用程式移除應用程式 Proxy 設定，而且可以完全刪除應用程式（如果有指定的話）。</span><span class="sxs-lookup"><span data-stu-id="ab078-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="ab078-110">您可以使用 PowerShell **還原已刪除的應用程式** 。</span><span class="sxs-lookup"><span data-stu-id="ab078-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="ab078-111">在您想要還原的應用程式被識別後，您可以使用 [AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)還原它。</span><span class="sxs-lookup"><span data-stu-id="ab078-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
