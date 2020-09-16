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
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745299"
---
# <a name="configure-files-on-demand"></a>設定 [檔案隨選]

OneDrive [檔案隨選] 能協助您存取 OneDrive 中的所有檔案，而不必全部下載並占用您裝置上的儲存空間。

若要在您的電腦上設定 [檔案隨選]：

1. 選取 Windows 工作列通知區域中的藍色 **OneDrive** 雲朵圖示。 選取 **[說明與設定]** 齒輪圖示 > **[設定]**。
2. 在 **[設定]** 索引標籤上，選取 **[節省空間並在使用的同時下載檔案]** 方塊。  

您也可以使用登錄設定 [檔案隨選]。

如果停用此設定，Windows 10 使用者會與 Windows 舊版使用者有相同的同步處理行為，且將無法開啟檔案隨選。 如果不設定此設定，使用者可以開啟或關閉檔案檔案隨選。

啟用此原則會將下列登錄機碼值設為 1。 停用此原則會將下列登錄機碼值設為 0。

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

若您無法在 [設定] 中看見 [檔案隨選]，請確認服務 "Windows Cloud Files Filter Driver" 的啟動類型設定為 2 (AUTO_START)。 啟用此功能會將下列登錄機碼值設為 2。

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`