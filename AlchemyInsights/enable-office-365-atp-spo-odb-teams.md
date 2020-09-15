---
title: 為 SharePoint、OneDrive 和 Microsoft 團隊啟用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709898"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>針對 SharePoint 線上、OneDrive 和 Microsoft 團隊啟用 Office 365 的高級威脅防護

1. 移至 https://protection.office.com 並登入。
2. 選擇 [**威脅管理**  >  **原則**  >  **安全附件**]。
3. 選取 [ **開啟 SharePoint、OneDrive 和 Microsoft 小組的 ATP**]，然後按一下 [ **儲存**]。
4.  (建議) 成為全域系統管理員或 SharePoint Online 管理員，請執行 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將 **DisallowInfectedFileDownload** 參數設定為 *true*。
5.  (建議的) 設定偵測到的檔案 [警示](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 。

> [!NOTE]
> ATP 只會掃描 SharePoint Online、OneDrive 或 Microsoft 小組中的每一個檔案。 檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。 請參閱 [ATP 的 SharePoint、OneDrive 和 Microsoft 團隊](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。