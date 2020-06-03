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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506909"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>針對 SharePoint 線上、OneDrive 和 Microsoft 團隊啟用 Office 365 的高級威脅防護

1. 移至 https://protection.office.com 並登入。
2. 選擇 [**威脅管理**  >  **原則**  >  **安全附件**]。
3. 選取 [**開啟 SharePoint、OneDrive 和 Microsoft 小組的 ATP**]，然後按一下 [**儲存**]。
4. 推薦以全域管理員或 SharePoint 線上管理員身分執行[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將**DisallowInfectedFileDownload**參數設定為*true*。
5. 推薦[設定](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)偵測到的檔案的警示。

> [!NOTE]
> ATP 只會掃描 SharePoint Online、OneDrive 或 Microsoft 小組中的每一個檔案。 檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。 請參閱[ATP 的 SharePoint、OneDrive 和 Microsoft 團隊](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。