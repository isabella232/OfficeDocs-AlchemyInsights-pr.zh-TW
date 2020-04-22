---
title: 傳統 SharePoint 的審計記錄報告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3270f1ab03bacb235cbdc3d710053c858f0a5183
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43741956"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint 和 OneDrive 審核記錄檔

## <a name="sharepoint-classic-audit-logs"></a>SharePoint 傳統的審計記錄

SPO 舊版審核已遷移至整合的審計記錄檔（UAL）。 所有 SPO 的舊版審核報告現在都會透過 UAL 供電，舊版的審核信號也會遷移至 UAL。

主要變更：

* 無法使用修整功能。
* 無法使用選擇要進行審核的特定事件。 請參閱[本檔](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)，以取得預設可供使用之審核事件的完整清單。
* 無法使用 [**自訂報告**] 底下的 [**位置**] 選項。
* 無法使用「**開啟或下載檔案**的事件] 選項。

[設定網站集合的審核設定](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>從相容性中 SharePoint 和 OneDrive 現代化的整合審計記錄檔

* [開啟/關閉整合的審計記錄](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

SharePoint 或 OneDrive 中不需要進行其他設定。

使用「審核記錄搜尋」檢查檔案的活動、資料夾（s）、使用者的許可權：

* [檔案和頁面活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [資料夾活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [共用及存取要求活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [同步處理活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [網站管理活動](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

如需如何取得這些事件的詳細資訊，請參閱[搜尋審核記錄](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)檔。
