---
title: 在 SharePoint Online 中建立網站
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 9ab06cbd1648da31d8a04e61c237a2326b4bbe93
ms.sourcegitcommit: f856d46a325c517fc29d935c27f21b77c4219e66
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/24/2019
ms.locfileid: "35199264"
---
# <a name="create-sharepoint-sites-using-templates"></a>使用範本建立 SharePoint 網站

SharePoint 網站範本是專為特定業務需求而設計的預置定義。 如需詳細資訊, 請參閱[使用範本建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。

以下是有關在 Sharepoint Online 中將網站或清單儲存為範本的一些常見問題/解決方案。 

**[儲存網站/清單範本] 按鈕無法使用或遺失**

系統管理員必須允許自訂腳本啟用範本功能。 如需詳細步驟, 請參閱 

- [允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 不支援 [另存網站為範本] 命令, 而且可能會在使用 SharePoint Server 發佈基礎結構的網站上造成問題。

**無法建立或無法正常運作網站範本**

範本可能遺失[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)且不會啟動。 如果無法在目前的網站集合中啟用此功能, 您就無法使用網站範本來建立網站。

- 檢查是否有任何清單或文件庫超出5000個專案的[清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59), 因為這會封鎖網站範本的建立。

- 網站可能使用太多資源, 因此網站範本超過 50 MB 的限制。


- 顯示使用查閱欄之清單中的資料時發生問題。 如需詳細資訊, 請參閱[範本產生的清單不會在 SharePoint Online 中顯示正確查閱清單中的資料](https://support.office.com/article/template-generated-list-doesn-t-display-correct-data-for-a-column-in-sharepoint-online-20430b62-e40c-4f6f-8889-aa24e80d605a)。

如需常見問題和解決方案的詳細資訊, 請參閱[Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。



