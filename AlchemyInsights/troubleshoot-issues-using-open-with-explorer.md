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
ms.openlocfilehash: c95f07b9fb7251442577c014e4005dbe3f92ceb4
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29661742"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="d731b-102">修正檔案總管開啟的問題</span><span class="sxs-lookup"><span data-stu-id="d731b-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="d731b-103">修正 SharePoint 或使用 [**檔案總管中開啟**] 命令的 OneDrive 中開啟文件庫的一般問題：</span><span class="sxs-lookup"><span data-stu-id="d731b-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="d731b-p101">使用 Internet Explorer 10 或 Internet Explorer 11。**檔案總管中開啟**不相容於 Microsoft Edge、 Google Chrome、 Firefox 與其他人。**檔案總管中開啟**已停用 Internet Explorer 以外的所有瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="d731b-p101">Use Internet Explorer 10 or Internet Explorer 11. **Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others. **Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="d731b-p102">**檔案總管中開啟**並不提供 SharePoint 文件庫的現代體驗。而是使用**中檔案總管檢視**。選取 [**檢視選項** \> **檔案總管] 中的檢視**。在檔案總管] 中的檢視不相容於 Microsoft Edge、 Google Chrome、 Firefox 與其他人。在**檔案總管] 中的檢視**只能在 Internet Explorer。</span><span class="sxs-lookup"><span data-stu-id="d731b-p102">**Open with Explorer** is not available in the modern experience for SharePoint libraries. Use **View in File Explorer** instead. Select **View options** \> **View in File Explorer**. View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others. **View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="d731b-p103">請確定執行 WebClient 服務。在 Windows 搜尋] 方塊中，輸入執行，請選取 [執行桌面應用程式、 輸入 services.msc，並按 Enter。捲動到 WebClient 服務，並確定 [**狀態**] 欄會顯示 「 執行 」。如果它不連按兩下 [服務、 按一下 [**開始**] 及 [**確定]**。（您可能需要先啟用服務的 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**）。</span><span class="sxs-lookup"><span data-stu-id="d731b-p103">Make sure the WebClient service is running. In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter. Scroll down to the WebClient service and make sure the **Status** column displays "Running." If it doesn't, double-click the service, click **Start**, and then click **OK**. (You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="d731b-p104">如果您要複製或移動多個檔案及資料夾之後，但如果您想要在文件庫中定期工作方便使用中檔案總管] 中開啟文件庫，建議次它。若要疑難排解在檔案總管] 中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。如需設定同步處理的資訊，請參閱 ＜[具有新 OneDrive sync 用戶端的同步處理 SharePoint 檔案](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="d731b-p104">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it. To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="d731b-120">請參閱 ＜[如何使用 「 開啟與檔案總管 」 命令來疑難排解 SharePoint Online 中的問題](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="d731b-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4) for more information.</span></span> 
  

