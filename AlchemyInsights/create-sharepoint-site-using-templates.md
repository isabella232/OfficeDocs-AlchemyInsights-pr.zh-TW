---
title: 在 SharePoint Online 中建立網站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: 458990889d3c074820527982cbfa6e2d198d3e66
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052460"
---
# <a name="create-sharepoint-sites-using-templates"></a>建立 SharePoint 網站使用範本

SharePoint 網站範本是預先的定義專為特定的業務需求。 如需詳細資訊，請參閱[使用範本來建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。

以下是一些常見的問題/解決方案有關儲存網站或清單作為範本，在 Sharepoint Online 中。 

**儲存網站/清單範本] 按鈕不提供或遺失**

系統管理員就必須允許自訂指令碼來啟用範本的功能。 如需詳細步驟，範例和考量請參閱 

- [允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 另存網站為範本] 命令不支援，及使用 SharePoint Server 發佈基礎結構的網站上可能會造成問題。

**[網站] 範本無法建立或無法正常運作**

範本可能會遺失的[功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx)，並不會啟動。 如果找不到可在目前的網站集合中啟動的功能，您無法使用網站範本建立網站。

- 請查看是否任何清單或文件庫超過 5000 的項目[清單檢視的限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)為這可以封鎖架設的網站範本。

- 網站使用太多的資源並因此網站範本超過 50 MB 的限制。


- 有問題，顯示使用查閱欄的清單中的資料。 如需詳細資訊，請參閱[範本產生清單不會顯示來自 SharePoint Online 中正確的查閱清單的資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。

針對常見的問題與解決方案的詳細資訊，請檢查[建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。



