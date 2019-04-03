---
title: 啟用 Office 365 ATP SharePoint、 OneDrive 及 Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030902"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>啟用 SharePoint Online、 OneDrive 及 Microsoft Teams 的 Office 365 進階的威脅防護

1. 移至 [https://protection.office.com並登入。
2. 選擇 [**威脅管理** > **原則** > **安全附件**。
3. 選取 [**開啟 ATP SharePoint、 OneDrive 及 Microsoft Teams**，，然後按一下 [**儲存**。
4. （建議使用）以全域管理員或 SharePoint Online 系統管理員，執行[Set-spotenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps)指令程式搭配**DisallowInfectedFileDownload**參數設為*true*。
5. （建議使用）[設定提醒](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files)偵測到的檔案。

> [!NOTE]
> ATP 會 nto 掃描 SharePoint Online、 OneDrive 或 Microsoft Teams 中每一個檔案。 掃描檔案有以非同步方式，透過使用共用和來賓活動事件，以及智慧啟發和威脅訊號，以識別惡意檔案的程序。 請參閱[https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。