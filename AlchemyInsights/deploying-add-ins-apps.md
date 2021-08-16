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
ms.openlocfilehash: 3aacc3c6675f4102a5b34a435c862215dbfd0479b75549d608ed3c91021ed3d7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031397"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>部署 Microsoft 365 Apps 的增益集

集中式部署是將 Office 增益集部署至組織內之使用者和群組的建議方法。 若要部署增益集，請遵循下列步驟：

**附注：** 若要以個別使用者的身分安裝 Office 增益集，請參閱 [在 Office 程式中查看、管理及安裝增益集](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)。 此外，請確定已啟用個別購買 Office 儲存區增益集。 如需詳細資訊，請參閱[除了 Outlook) 以外，關閉所有用戶端上的 Office 儲存區，以避免增益集下載 (](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)。

1. 確定您的環境符合使用集中式部署來部署增益集的需求。 如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements)。
2. 移至 **設定**  >  的 **整合式應用程式**  >  在 Microsoft 365 系統管理中心中 **取得應用程式** 以部署增益集。 

附註： 

- 整合式應用程式需要管理員具備全域管理員或 Exchange 系統管理員許可權。

- 當您將增益集部署至多個使用者時，建議您使用群組而不是個別使用者來進行工作分派。 如需詳細資訊，請參閱 [將增益集指派給使用者和群組時的考慮](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)。

- 集中式部署不支援具有父群組之嵌套群組或群組中的使用者。 如需詳細資訊，請參閱 [使用者和群組指派](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)。

- 確定已啟用 Microsoft 365 App Management Service (GUID: ' 0517ffae-825d-4aff-999e-3f2336b8a20a ' ) 以供使用者登入。 如需詳細資訊，請參閱 [設定應用程式屬性](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)。

- 如果您使用整合式應用程式來部署增益集時遇到問題，請嘗試使用 [增益集](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)進行部署。

如需詳細資訊，請參閱：

[在系統管理中心](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 部署增益集[管理管理中心](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 內的增益集[使用集中式部署 PowerShell Cmdlet 來管理增益集](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
透過[Microsoft 365 系統管理中心使用集中式部署來發佈 Office 增益集](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
[疑難排解：使用者未看到增益集](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
[疑難排解 Office 增益集的使用者錯誤](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)