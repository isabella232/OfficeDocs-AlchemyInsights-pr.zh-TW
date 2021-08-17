---
title: 設定檔同步處理
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320700"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>我的設定檔變更何時同步處理至 SharePoint 的使用者設定檔應用程式？

SharePoint線上使用 Active Directory 匯入計時器工作 (AD 匯入) ，將使用者和群組匯入使用者設定檔應用程式。 
  
1. AD 匯入將 SharePoint 線上目錄存放區中的變更同步處理至使用者設定檔應用程式。 這些變更會以批次處理。
    
2. 計時器工作會在同步處理變更之前執行。
    
**附注**：執行工作所需的時間取決於要處理的變更數目。 大量的變更所需的時間較長。 服務等級協定 (SLA) 指出 SharePoint Online 目錄中的使用者變更會在使用者設定檔應用程式中，于24小時內反映。 
  
[SharePoint Online 中使用者設定檔同步處理的詳細資訊](https://go.microsoft.com/fwlink/?linkid=875671)
  

