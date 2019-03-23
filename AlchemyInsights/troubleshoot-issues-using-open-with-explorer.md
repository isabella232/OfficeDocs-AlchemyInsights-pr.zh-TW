---
title: 使用檔案總管中開啟的問題進行疑難排解
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 03bb3ad01a716390ec50845b29ddf6cc81a83116
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30759285"
---
# <a name="fix-problems-with-open-with-explorer"></a>修正問題的檔案總管中開啟

修正在 SharePoint 或 OneDrive 使用**檔案總管中開啟**的命令中開啟的文件庫的一般問題： 
  
- 使用 Internet Explorer 10 或 Internet Explorer 11。 **檔案總管中開啟**不是與 Microsoft Edge、 Google Chrome、 Firefox 和其他相容。 **檔案總管中開啟**已停用 Internet Explorer 以外的所有瀏覽器中。 
    
- **開啟檔案總管**中沒有 SharePoint 文件庫的新式體驗。 改為使用**中檔案總管] 檢視**。 選取 [**檢視選項** \> **檔案總管] 中的檢視**。 在檔案總管] 中的檢視不是與 Microsoft Edge、 Google Chrome、 Firefox 和其他相容。 在 [**檔案總管] 中的檢視**只能在 Internet Explorer 中使用。 
    
- 請確定 WebClient 服務正在執行。 在 [Windows 搜尋方塊中，輸入執行，請選取執行桌面應用程式，輸入 services.msc，，然後按 Enter 鍵。 捲動至 WebClient 服務，並確定 [**狀態**] 欄會顯示 「 執行 」。 如果沒有，按兩下 [服務] 按一下 [**開始**]，然後按一下 [**確定]**。 （您可能需要先選取 [**啟動類型**] 方塊中的 [**手動**] 或 [**自動**啟用服務）。 
    
> [!NOTE]
> 在檔案總管中開啟文件庫很方便如果您要複製或移動多個檔案和資料夾之後，但如果您想要定期處理程式庫中，建議您同步處理它。 若要疑難排解在檔案總管中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。 如需設定同步處理的資訊，請參閱 <<c0>同步處理 SharePoint 檔案與新的 OneDrive 同步處理用戶端。
  
請參閱如需詳細資訊的文章[如何使用 「 開啟與檔案總管 」 命令，以在 SharePoint Online 中的問題進行疑難排解](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)。 
  

