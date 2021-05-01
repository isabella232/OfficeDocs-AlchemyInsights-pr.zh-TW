---
title: 部署 Microsoft 365 Apps 的增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/30/2021
ms.locfileid: "52107509"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="cb92e-102">部署 Microsoft 365 Apps 的增益集</span><span class="sxs-lookup"><span data-stu-id="cb92e-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="cb92e-103">集中式部署是將 Office 增益集部署至組織內之使用者和群組的建議方法。</span><span class="sxs-lookup"><span data-stu-id="cb92e-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="cb92e-104">若要部署增益集，請遵循下列步驟：</span><span class="sxs-lookup"><span data-stu-id="cb92e-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="cb92e-105">**附注：** 若要以個別使用者的身分安裝 Office 增益集，請參閱 [在 Office 程式中查看、管理及安裝增益集](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)。</span><span class="sxs-lookup"><span data-stu-id="cb92e-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="cb92e-106">此外，請確定已啟用個別購買 Office 儲存區增益集。</span><span class="sxs-lookup"><span data-stu-id="cb92e-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="cb92e-107">確定您的環境符合使用集中式部署來部署增益集的需求。</span><span class="sxs-lookup"><span data-stu-id="cb92e-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="cb92e-108">如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)。</span><span class="sxs-lookup"><span data-stu-id="cb92e-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="cb92e-109">移至 **設定**  >  的 **整合式應用程式**  >  在 Microsoft 365 系統管理中心 **取得應用程式**，以部署增益集。</span><span class="sxs-lookup"><span data-stu-id="cb92e-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="cb92e-110">附註：</span><span class="sxs-lookup"><span data-stu-id="cb92e-110">Notes:</span></span> 

- <span data-ttu-id="cb92e-111">整合式應用程式需要管理員具備全域管理員或 Exchange 系統管理員許可權。</span><span class="sxs-lookup"><span data-stu-id="cb92e-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="cb92e-112">當您將增益集部署至多個使用者時，建議您使用群組而不是個別使用者來進行工作分派。</span><span class="sxs-lookup"><span data-stu-id="cb92e-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="cb92e-113">如需詳細資訊，請參閱 [將增益集指派給使用者和群組時的考慮](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)。</span><span class="sxs-lookup"><span data-stu-id="cb92e-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="cb92e-114">集中式部署不支援具有父群組之嵌套群組或群組中的使用者。</span><span class="sxs-lookup"><span data-stu-id="cb92e-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="cb92e-115">如需詳細資訊，請參閱 [使用者和群組指派](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)。</span><span class="sxs-lookup"><span data-stu-id="cb92e-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="cb92e-116">確定已啟用 Microsoft 365 App Management Service (GUID: ' 0517ffae-825d-4aff-999e-3f2336b8a20a ' ) 以供使用者登入。</span><span class="sxs-lookup"><span data-stu-id="cb92e-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="cb92e-117">如需詳細資訊，請參閱 [設定應用程式屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)。</span><span class="sxs-lookup"><span data-stu-id="cb92e-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="cb92e-118">如果您使用整合式應用程式來部署增益集時遇到問題，請嘗試使用 [增益集](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)進行部署。</span><span class="sxs-lookup"><span data-stu-id="cb92e-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="cb92e-119">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="cb92e-119">For more information, see:</span></span>

<span data-ttu-id="cb92e-120">[在系統管理中心](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 部署增益集[管理管理中心](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 內的增益集[使用集中式部署 PowerShell Cmdlet 來管理增益集](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
透過[Microsoft 365 系統管理中心，使用集中式部署來發佈 Office 增益集](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
[疑難排解：使用者未看到增益集](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
[疑難排解 Office 增益集的使用者錯誤](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="cb92e-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>