---
title: 使用 [以瀏覽器開啟] 疑難排解問題
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323557"
---
# <a name="fix-problems-with-open-with-explorer"></a>修正使用 Explorer 開啟的問題

修正使用 [**使用 [使用 [開啟] 瀏覽器** 命令在 SharePoint 或 OneDrive 中開啟文件庫時發生的常見問題： 
  
- 使用 Internet Explorer 10 或 Internet Explorer 11。 **使用 Explorer 開啟** 與 Microsoft Edge、Google Chrome、Firefox 及其他使用者不相容。 在 Internet Explorer 以外的所有瀏覽器中停 **用 Explorer 開啟**。 
    
- 在 SharePoint 文件庫的現代體驗中，無法使用 **Explorer 開啟**。 請改 **為在檔案資源管理器中使用 View** 。 選取檔案 \> **瀏覽器中的**[view options view]。 檔案瀏覽器中的視圖與 Microsoft Edge、Google Chrome、Firefox 及其他使用者不相容。 僅能在 Internet Explorer 中 **查看檔案資源管理器** 中的。 
    
- 請確定 WebClient 服務正在執行中。 在 [Windows 搜尋] 方塊中，輸入 run，選取 [執行桌面應用程式]，輸入 services.msc，然後按 enter。 向中向左下到 WebClient 服務，確定 [ **狀態** ] 欄顯示 "執行]。 如果不是，請按兩下服務，按一下 [ **開始**]，然後按一下 **[確定]**。  (您可能需要先在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**]，以啟用服務。 )  
    
**附注**：如果您需要將多個檔案和資料夾複製或移動一次，但是如果您想要定期在文件庫中工作，則在檔案瀏覽器中開啟文件庫是很便利的方式，我們建議您同步處理。 若要疑難排解在檔案瀏覽器中開啟的問題，請參閱 [在瀏覽器中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。 如需設定同步處理的詳細資訊，請參閱[sync SharePoint files with new OneDrive 同步處理 client](https://go.microsoft.com/fwlink/?linkid=871666)。
  
如需詳細資訊，請參閱[如何使用「開啟 with Explorer」命令來疑難排解 SharePoint Online 中的問題](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)。 
  

