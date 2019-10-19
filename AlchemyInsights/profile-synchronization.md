---
title: 設定檔同步處理
ms.author: arnek
author: arnek
ms.date: 6/20/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b9b90dad6c5fa41afcd4e4c9a929594735eca066
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36554324"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>何時執行動作我的設定檔變更同步處理至 SharePoint 使用者設定檔應用程式？

SharePoint Online 會使用 Active Directory 匯入計時器服務 （AD 匯入） 匯入至使用者設定檔應用程式的使用者和群組。 
  
1. AD 匯入同步使用者設定檔應用程式從 SharePoint Online 目錄存放區的變更。 這些變更會分批處理。
    
2. 計時器工作執行之前所做的變更會同步處理。
    
> [!NOTE]
> 要執行的工作所花費的時間取決於變更處理程序數目。 大量變更耗時越久。 服務層級協議 (SLA) 會指出使用者在 SharePoint Online 目錄中的變更會反映使用者設定檔應用程式中，在 24 小時內。 
  
[在 SharePoint Online 中的使用者設定檔同步處理的詳細資訊](https://go.microsoft.com/fwlink/?linkid=875671)
  

