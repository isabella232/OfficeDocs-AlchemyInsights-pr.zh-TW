---
title: 在 SharePoint Online 中建立網站
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732205"
---
# <a name="create-sharepoint-sites-using-templates"></a>使用範本建立 SharePoint 網站

新式通訊或小組網站不支援將網站儲存為範本的功能。 如需使用範本的詳細資訊 [，請參閱儲存、下載和上傳 SharePoint 網站為範本](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template)。

以下是一些有關在 Sharepoint Online 中將網站或清單儲存為範本的常見問題/解決方案。 

**無法使用或遺漏 [儲存網站/清單範本] 按鈕**

系統管理員必須允許自訂腳本啟用範本功能。 如需詳細步驟，請參閱 

- [允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- [另存網站為範本] 命令不受支援，而且可能會導致使用 SharePoint 伺服器發佈基礎結構之網站的問題。

**無法建立或無法正常運作的網站範本**

範本可能遺漏了某 [項功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ，且無法啟動。 如果無法在目前的網站集合中啟動該功能，您就無法使用網站範本來建立網站。

- 檢查是否有任何清單或文件庫超出5000個專案的 [清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ，因為這會封鎖網站範本的建立。

- 網站可能使用太多資源，因此網站範本超過 50 MB 的限制。


- 使用查閱欄的清單顯示資料時出現問題。 如需詳細資訊，請參閱 [範本產生的清單，在 SharePoint Online 中不會顯示正確查閱清單中的資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。

如需有關常見問題和解決方案的詳細資訊，請參閱 [建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。



