---
title: 啟用 SharePoint、OneDrive 和 Microsoft Teams 的 Office 365 ATP
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
ms.openlocfilehash: 4a29fdf1b61dd51b85793a1346bea193c67f70d32344470cb5449cf767da4a24
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896594"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>針對 SharePoint 線上、OneDrive 和 Microsoft Teams 啟用 Microsoft Defender Office 365

1. 移至 https://protection.office.com 並登入。
2. 選擇 **威脅管理**  >  **原則**  >  **保管庫附件**。
3. **針對 SharePoint、OneDrive 及 Microsoft Teams，選取 [為 Office 365 開啟 Defender**]，然後按一下 [**儲存**]。
4.  (建議) 成為全域系統管理員或 SharePoint Online 管理員，請執行 [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) Cmdlet，並將 **DisallowInfectedFileDownload** 參數設定為 *true*。
5.  (建議的) 設定偵測到的檔案 [警示](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) 。

> [!NOTE]
> Microsoft Defender for Office 365 不會掃描 SharePoint Online、OneDrive 或 Microsoft Teams 中的每一個檔案。 檔案會透過使用共用和來賓活動事件的處理常式進行非同步掃描，並使用智慧試探法和威脅信號來識別惡意檔。 請參閱適用[于 SharePoint、OneDrive 和 Microsoft Teams 的 Microsoft Defender Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。