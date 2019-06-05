---
title: 將群組新增至 SharePoint 網站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 352bad1b8fe219f95a37c9ac268c6c4dd8801dfc
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719473"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a>在 SharePoint Online 中建立群組連線的網站

<p><strong>有幾個常見的問題發生時建立或重新建立一組連線網站。&nbsp;</strong></p>  <p>1.如果您已刪除的群組和其連線的網站，並想要使用相同的 URL 建立另一個網站，您需要永久移除舊的網站。</p>  <ul>  <li>下載<a title="SPO 管理命令介面" href="https://support.office.com/en-ie/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429">SPO 管理命令介面</a> - powershell 快速入門的詳細資訊，請參閱<a title="開始使用 SharePoint Online 管理命令介面" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">開始使用 SharePoint Online 管理命令介面</a>。 <br /><br /></li>  <li>移除網站刪除網站使用<a title="Remove-spodeletedsite" href="https://docs.microsoft.com/en-us/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps">Remove-spodeletedsite</a> powershell cmdlet。</li>  </ul>  <p>如果您要建立群組連線的網站，並收到警告<strong>'另一個群組別名相同但已經存在'</strong>，檢查從現有的群組<a title="從管理中心的 Office 365" href="https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups">Office 365 系統管理中心從</a>。 若要解決此問題，如果不再需要刪除現有的群組或使用不同的別名建立網站指派。&nbsp;</p>  <p><strong>有不同的方式來建立，與 SharePoint 使用新式群組。&nbsp;</strong></p>  <ol>  <li>您可以將現有網站連線至 Office 365 群組。 如需詳細資訊，請參閱<a title="連線使用 SharePoint 使用者 ineterface Office 365 群組" href="https://docs.microsoft.com/en-us/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface">連線 Office 365 群組使用 SharePoint 使用者 ineterface</a>。</li>  <li>若要建立 Office 365 群組連線的網站，您需要建立小組網站。 如需詳細資訊，請參閱<a title="SharePoint 中建立小組網站" href="https://support.office.com/en-us/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d">在 SharePoint 中建立小組網站。</a></li>  </ol>

