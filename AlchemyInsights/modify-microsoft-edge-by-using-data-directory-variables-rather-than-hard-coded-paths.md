---
title: 使用資料目錄變數 (而非硬式編碼路徑) 修改 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8222"
- "9004596"
ms.openlocfilehash: 23ce69157c465c56d0fc5ada7c2c159e3192fd75
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897491"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>使用資料目錄變數 (而非硬式編碼路徑) 修改 Microsoft Edge

例如，在 Windows 上若要將設定檔資料儲存在使用者的本機應用程式資料下，而非預設位置中，請將 *UserDataDir* 原則設定為 **${local_app_data}\Edge\Profile**。

如需詳細資訊，請參閱[建立 Microsoft Edge 使用者資料目錄變數](https://docs.microsoft.com/deployedge/microsoft-edge-policies)。