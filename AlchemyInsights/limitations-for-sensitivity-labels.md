---
title: 對 SharePoint 和 OneDrive 中的 Office 檔案啟用敏感度標籤的限制
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e2fc8fcf27eb916f64e4235cd116d9a7096e6078391e72363421ac3de721f5ee
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899755"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>對 SharePoint 和 OneDrive 中的 Office 檔案啟用敏感度標籤的限制

在 SharePoint 和 OneDrive 中啟用 Office 檔案的敏感度標籤時，請注意需求和限制，包括：

- 當檔案包含 PowerQuery 資料、透過自訂的附加元件或自訂 XML 元件所儲存的資料時，SharePoint 和 OneDrive 無法處理某些從 Office 桌面應用程式標示和加密的檔案。
- SharePoint 和 OneDrive 不會將敏感度標籤自動套用至已使用 Azure 資訊保護 (AIP) 標籤加密的現有檔案。若要將敏感度標籤套用至加密檔案： 
    - 確認已將 AIP 標籤移轉和發佈到 Microsoft 365 合規性中心。
    - 下載已加標籤的檔案，然後將檔案上傳到原始 SharePoint 或 OneDrive 位置。
- 對於加密的檔案，不支援列印。

如需限制的其它詳細資訊，請參閱 [對 SharePoint 和 OneDrive 中的 Office 檔案啟用敏感度標籤](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)。
