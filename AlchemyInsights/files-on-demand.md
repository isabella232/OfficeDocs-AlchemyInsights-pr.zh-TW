---
title: 檔案隨選
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 10efdb5e1a90b3e279b8e1716e66a544d0ee34465245f5670930d8a9364a8cc3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53977432"
---
# <a name="configure-files-on-demand"></a>設定 [檔案隨選]

[OneDrive 檔案隨選] 需要 [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040)（版本 1709 或更新版本）或 Windows Server 2019 及 OneDrive 組建 17.3.7064.1005 或更新版本。

OneDrive [檔案隨選] 能協助您存取 OneDrive 中的所有檔案，而不必全部下載並占用您裝置上的儲存空間。

若要在您的電腦上設定 [檔案隨選]：

1. 選取 Windows 工作列通知區域中的藍色 **OneDrive** 雲朵圖示。 選取 **[說明與設定]** 齒輪圖示 > **[設定]**。
2. 在 **[設定]** 索引標籤上，選取 **[節省空間並在使用的同時下載檔案]** 方塊。  

您也可以使用登錄設定 [檔案隨選]。

如果停用此設定，Windows 10 使用者會與 Windows 舊版使用者有相同的同步處理行為，且將無法開啟檔案隨選。如果不設定此設定，使用者可以開啟或關閉檔案檔案隨選。

啟用此原則會將下列登錄機碼值設為 1。 停用此原則會將下列登錄機碼值設為 0。

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

若您無法在 [設定] 中看見 [檔案隨選]，請確認服務 "Windows Cloud Files Filter Driver" 的啟動類型設定為 2 (AUTO_START)。啟用此功能會將下列登錄機碼值設為 2。

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`