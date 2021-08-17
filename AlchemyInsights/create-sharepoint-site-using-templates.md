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
ms.openlocfilehash: eaf09aebad5568aab3a716ce28c8ce3357c9f43175e1b1458bfcd43fd95a71fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057957"
---
# <a name="create-sharepoint-sites-using-templates"></a>使用範本建立 SharePoint 網站

新式通訊或小組網站不支援將網站另存為範本的功能。 如需關於使用範本的詳細資訊，請參閱[儲存、下載，然後上傳 SharePoint 網站做為範本](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template) (英文)。

以下是一些有關在 Sharepoint Online 中將網站或清單儲存為範本的常見問題/解決方案。 

**無法使用或遺漏 [儲存網站/清單範本] 按鈕**

系統管理員必須允許自訂指令碼以啟用範本功能。 如需詳細步驟，請參閱 

- [允許或防止自訂指令碼](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- 不支援 [另存網站為範本] 命令，可能會導致使用 SharePoint 伺服器發佈基礎結構的網站發生問題。

**無法建立或無法正常運作的網站範本**

範本可能遺漏了某 [項功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ，且無法啟動。 如果目前網站集合中無法啟用該功能，則無法使用網站範本創建網站。

- 檢查是否有任何清單或文件庫超過[清單檢視限制閾值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59)的 5000 個項目限制，因為這會導致網站範本無法建立。

- 網站可能使用了太多資源，因此網站範本超出了50 MB 的限制。


- 顯示使用查閱欄的清單中的資料時出現問題。 如需詳細資訊，請參閱[範本產生的清單在 SharePoint Online 中無法從正確的查閱清單顯示資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。

如需有關常見問題和解決方案的詳細資訊，請參閱 [建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。



