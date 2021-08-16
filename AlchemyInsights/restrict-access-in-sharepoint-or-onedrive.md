---
title: 在 SharePoint 或 OneDrive 中限制存取權
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075031"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>在 SharePoint 或 OneDrive 中限制存取權

在 SharePoint 和 OneDrive 中，您可以只將存取權授與您想要存取的群組或個人，來限制存取檔、資料夾和清單等專案。 根據預設，SharePoint 中的許可權會從階層中較高的位置繼承。 因此，檔案會從該資料夾繼承其許可權，該資料夾會從該資料夾繼承其許可權，而這些許可權會從該網站繼承許可權。
  
您可以在較高的層級進行共用 (例如，共用整個網站) 然後中斷繼承（如果您不想共用網站上的所有專案）。 不過，我們不建議您這麼做，因為它會使許可權在未來變得更複雜且令人困惑。 以下是您可以執行的動作：
  
- 例如，如果您想要共用資料夾中除了一個檔案之外的所有內容，請將該檔案移至未共用的新位置。
    
- 如果資料夾中有兩個子資料夾，而且想要與群組 A 和 B 共用一個子資料夾，而且只允許群組存取第二個子資料夾，請與群組 A 共用父項資料夾，並將 B 群組新增至第一個子資料夾。
    
[停止共用檔案或資料夾 ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

