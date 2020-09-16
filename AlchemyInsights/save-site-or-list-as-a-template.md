---
title: 將網站或清單另存為範本
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727522"
---
# <a name="save-site-or-list-as-a-template"></a>將網站或清單另存為範本

SharePoint 網站範本是針對特定商務需求所設計的預置定義。 如需詳細資訊，請參閱 [使用範本建立不同類型的 SharePoint 網站](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4)。

以下是一些常見的問題/解決方案，有關將網站或清單儲存為 SharePoint 線上中的範本。

**無法使用或遺漏 [儲存網站/清單範本] 按鈕**。 

- 系統管理員必須允許自訂腳本啟用範本功能。 如需詳細步驟，請參閱 [Allow 或預防自訂腳本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。


- [另存網站為範本] 命令不受支援，而且可能會導致使用 SharePoint 伺服器發佈基礎結構之網站的問題。


**無法建立或無法正常運作的網站範本**

- 範本可能遺漏了某 [項功能](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) ，且無法啟動。 如果無法在目前的網站集合中啟動該功能，您就無法使用網站範本來建立網站。


- 檢查是否有任何清單或文件庫超出5000個專案的 [清單查看限制臨界值](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) ，因為這會封鎖網站範本的建立。


- 網站可能使用太多資源，因此網站範本超過 50 mb (MB) 限制。


- 使用查閱欄的清單顯示資料時出現問題。 如需詳細資訊，請參閱 [範本產生的清單，在 SharePoint Online 中不會顯示正確查閱清單中的資料](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data)。


如需有關常見問題和解決方案的詳細資訊，請參閱 [建立及使用網站範本](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989)。

