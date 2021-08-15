---
title: 使用 Explorer 開啟無法運作
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011327"
---
# <a name="open-with-explorer-isnt-working"></a>使用 Explorer 開啟無法運作

[ **開啟時使用 Explorer** ] 或 [檔案 **瀏覽器中的視圖** 無法運作請遵循下列 **步驟，確定** WebClient 服務已設定為執行]。 例如，當服務未執行時，可能需要很長的時間才能開啟 SharePoint 或 OneDrive 文件庫。 
  
1. 在 [Windows 搜尋] 方塊中，輸入 run，選取 [執行桌面應用程式]，輸入 services.msc，然後選取 **Enter**。
    
2. 向左下到 WebClient 服務，然後查看 [ **狀態** ] 欄。 如果 WebClient 服務 **狀態未執行，請** 按兩下服務，按一下 [ **開始**]，然後按一下 **[確定]**。 如有需要，請在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**]，以啟用服務。 
    
> [!NOTE]
> 若要疑難排解在檔案瀏覽器中開啟的問題，請參閱 [在瀏覽器中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。 探索同步處理做為更好的替代方法：[使用新的 OneDrive 同步處理用戶端同步處理 SharePoint](https://go.microsoft.com/fwlink/?linkid=871666)檔案。 
  

