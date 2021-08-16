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
ms.openlocfilehash: e3ad930ec79ef82f3bf95e84cb88e8bb9aea13637d8e59d845b486604664b137
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53992282"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hard-coded-paths"></a>使用資料目錄變數 (而非硬式編碼路徑) 修改 Microsoft Edge

例如，在 Windows 上若要將設定檔資料儲存在使用者的本機應用程式資料下，而非預設位置中，請將 *UserDataDir* 原則設定為 **${local_app_data}\Edge\Profile**。

如需詳細資訊，請參閱[建立 Microsoft Edge 使用者資料目錄變數](https://docs.microsoft.com/deployedge/microsoft-edge-policies)。