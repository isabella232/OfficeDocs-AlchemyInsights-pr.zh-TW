---
title: 使用資料目錄變數（而非硬編碼路徑）修改 Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "9003873"
- "6926"
ms.openlocfilehash: 235696d17711726da57d9a09c23b5b13140a28d7645299ef120a4b2c7b395c5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54113407"
---
# <a name="modify-microsoft-edge-by-using-data-directory-variables-rather-than-hardcoded-paths"></a>使用資料目錄變數（而非硬編碼路徑）修改 Microsoft Edge

例如，在 Windows 上若要將設定檔資料儲存在使用者的本機應用程式資料下，而非預設位置中，請將 **UserDataDir** 原則設定為 **${local_app_data}\Edge\Profile**。 

若要深入瞭解，請參閱[Create Microsoft Edge user data directory 變數](https://docs.microsoft.com/deployedge/edge-learnmore-create-user-directory-vars)。