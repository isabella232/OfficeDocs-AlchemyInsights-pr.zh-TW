---
title: 檔案總管中的開啟無法運作
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 73d33e50449345c312abdd39afcc36e0c95fd1c4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32419856"
---
# <a name="open-with-explorer-isnt-working"></a>檔案總管中的開啟無法正常運作

如果**開啟檔案總管**] 或 [**在檔案總管中的檢視**無法確定 WebClient 服務會設定為**執行**下列步驟。 例如，可能需要很長的時間，若要開啟的 SharePoint 或 OneDrive 文件庫，當服務未執行。 
  
1. 在 [Windows 搜尋方塊中，輸入執行，請選取 [執行桌面應用程式類型 services.msc，然後選取 [**輸入**]。
    
2. 捲動至 WebClient 服務，並檢查 [**狀態**] 欄。 如果 WebClient 服務狀態不**執行**，按兩下 [服務] 按一下 [**開始**]，然後按一下 [**確定]**。 如有需要選取 [**啟動類型**] 方塊中的 [**手動**] 或 [**自動**啟用 service]。 
    
> [!NOTE]
> 若要疑難排解在檔案總管中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。 瀏覽更好的另一種方法的同步處理：[同步處理 SharePoint 檔案與新的 OneDrive 同步處理用戶端](https://go.microsoft.com/fwlink/?linkid=871666)。 
  

