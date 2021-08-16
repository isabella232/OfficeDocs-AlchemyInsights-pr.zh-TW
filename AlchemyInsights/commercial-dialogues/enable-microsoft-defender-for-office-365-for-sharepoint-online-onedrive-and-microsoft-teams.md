---
title: 針對 SharePoint 線上、OneDrive 和 Microsoft Teams 啟用 Microsoft Defender Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058857"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>針對 SharePoint 線上、OneDrive 和 Microsoft Teams 啟用 Microsoft Defender Office 365

1. 使用您的全域系統管理員或安全性系統管理員認證，登入[Office 365 安全性與合規性中心](https://protection.office.com/)。
2. 在左窗格中選取 [**威脅管理**]，然後選取 [**原則**  >  [保管庫附件](https://protection.office.com/safeattachment)]。
3. **針對 SharePoint、OneDrive 及 Microsoft Teams，選取 [為 Office 365 開啟 Microsoft Defender**]，然後選取 [**儲存**]。
    > [!TIP]
    >
    > - 以全域管理員或 SharePoint Online 管理員身分執行下列 PowerShell Cmdlet，並將 **DisallowInfectedFileDownload** 參數設定為 *true*： [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [為偵測到的檔案設定警示](https://go.microsoft.com/fwlink/?linkid=2092110)

如需詳細資訊，請參閱適用[于 SharePoint、OneDrive 和 Microsoft Teams 的 Microsoft Defender Office 365](https://go.microsoft.com/fwlink/?linkid=2092041)。
