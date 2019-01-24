---
title: 疑難排解使用瀏覽器中開啟的問題
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 5be8a8f9f67939c7e2671855da259818269d9299
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29461071"
---
# <a name="fix-problems-with-open-with-explorer"></a>修正檔案總管開啟的問題

修正 SharePoint 或使用 [**檔案總管中開啟**] 命令的 OneDrive 中開啟文件庫的一般問題： 
  
- 使用 Internet Explorer 10 或 Internet Explorer 11。**檔案總管中開啟**不相容於 Microsoft Edge、 Google Chrome、 Firefox 與其他人。**檔案總管中開啟**已停用 Internet Explorer 以外的所有瀏覽器。 
    
- **檔案總管中開啟**並不提供 SharePoint 文件庫的現代體驗。而是使用**中檔案總管檢視**。選取 [**檢視選項** \> **檔案總管] 中的檢視**。在檔案總管] 中的檢視不相容於 Microsoft Edge、 Google Chrome、 Firefox 與其他人。在**檔案總管] 中的檢視**只能在 Internet Explorer。 
    
- 請確定執行 WebClient 服務。在 Windows 搜尋] 方塊中，輸入執行，請選取 [執行桌面應用程式、 輸入 services.msc，並按 Enter。捲動到 WebClient 服務，並確定 [**狀態**] 欄會顯示 「 執行 」。如果它不連按兩下 [服務、 按一下 [**開始**] 及 [**確定]**。（您可能需要先啟用服務的 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**）。 
    
> [!NOTE]
> 如果您要複製或移動多個檔案及資料夾之後，但如果您想要在文件庫中定期工作方便使用中檔案總管] 中開啟文件庫，建議次它。若要疑難排解在檔案總管] 中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。如需設定同步處理的資訊，請參閱 ＜[具有新 OneDrive sync 用戶端的同步處理 SharePoint 檔案](https://go.microsoft.com/fwlink/?linkid=871666)。
  
請參閱 ＜[如何使用 「 開啟與檔案總管 」 命令來疑難排解 SharePoint Online 中的問題](https://support.office.com/en-us/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)的詳細資訊。 
  

