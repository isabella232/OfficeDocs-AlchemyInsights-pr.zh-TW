---
title: 開啟瀏覽器未作用
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/10/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: b55fc7bd5670e655334ef7be368b245c8899633a
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278226"
---
# <a name="open-with-explorer-isnt-working"></a>開啟瀏覽器也無法正常運作

如果**檔案總管中開啟**或**檔案總管] 中的檢視**未作用務必 WebClient 服務設為**執行**遵循下列步驟。例如，可能需要長的時間才能開啟 SharePoint 或 OneDrive 文件庫時服務未執行。 
  
1. 在 Windows 搜尋] 方塊中，輸入執行，請選取 [執行桌面應用程式、 類型 services.msc 與然後選取 [ **Enter**。
    
2. 捲動到 WebClient 服務，並檢查 [**狀態**] 欄。如果 WebClient 服務狀態不**執行**，連按兩下 [服務、 按一下 [**開始**] 及 [**確定]**。必要時，在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**啟用服務]。 
    
> [!NOTE]
> 若要疑難排解在檔案總管] 中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。探索更好的替代項為同步處理：[同步處理 SharePoint 檔案與新 OneDrive sync 用戶端](https://go.microsoft.com/fwlink/?linkid=871666)。 
  

