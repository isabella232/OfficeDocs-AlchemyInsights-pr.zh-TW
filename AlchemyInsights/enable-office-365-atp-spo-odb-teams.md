---
title: 為 SharePoint、OneDrive 和 Microsoft 團隊啟用 Office 365 ATP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703417"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>針對 SharePoint 線上、OneDrive 和 Microsoft 團隊啟用 Office 365 的高級威脅防護

1. 移至 https://protection.office.com 並登入。
2. 選擇 [**威脅管理** > **原則** > **安全附件**]。
3. 選取 [**開啟 SharePoint、OneDrive 和 Microsoft 小組的 ATP**]，然後按一下 [**儲存**]。
4. 推薦以全域管理員或 SharePoint 線上管理員身分執行[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將**DisallowInfectedFileDownload**參數設定為*true*。
5. 推薦[設定](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)偵測到的檔案的警示。

> [!NOTE]
> ATP 只會掃描 SharePoint Online、OneDrive 或 Microsoft 小組中的每一個檔案。 檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。 請[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)參閱。