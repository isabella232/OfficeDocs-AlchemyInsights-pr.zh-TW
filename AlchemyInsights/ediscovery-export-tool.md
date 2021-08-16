---
title: eDiscovery 匯出工具
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: f7b7e1ae4f1f686fa510403d398c4ff750dbadb9065b8d63701a927eeac52d9b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101293"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>無法安裝或執行 eDiscovery 匯出工具？

如果您無法安裝或執行 eDiscovery 匯出工具來下載搜尋結果，請檢查下列事項：
  
- 您所使用的電腦符合下列先決條件：

  - 32或64位版本的 Windows 7 及更新版本

  - Microsoft .NET Framework 4.7

  - 支援的瀏覽器：

  - Microsoft Edge

    或者

  - Internet Explorer 10 和更新版本

    其他瀏覽器（如 Google Chrome 和 Mozilla Firefox）都不受支援。

- 您的組織可以連線到 Azure 中的端點，也就是 **\* blob.core.windows.net** (此萬用字元代表匯出工作) 的唯一識別碼。

- 您已在 Microsoft 365 安全性與合規性中心指派「匯出」角色 &amp; 。 根據預設，此角色只會指派給 eDiscovery 管理員角色群組。 請參閱 [指派 eDiscovery 許可權](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)。

如需詳細資訊，請參閱 [匯出內容搜尋結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)。

若要匯出的信箱超過10個，您必須使用下列 Powershell 下載匯出結果：  [從超過100k 的信箱匯出結果](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)。