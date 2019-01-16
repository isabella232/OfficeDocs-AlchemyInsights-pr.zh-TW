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
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="5c890-102">開啟瀏覽器也無法正常運作</span><span class="sxs-lookup"><span data-stu-id="5c890-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="5c890-p101">如果**檔案總管中開啟**或**檔案總管] 中的檢視**未作用務必 WebClient 服務設為**執行**遵循下列步驟。例如，可能需要長的時間才能開啟 SharePoint 或 OneDrive 文件庫時服務未執行。</span><span class="sxs-lookup"><span data-stu-id="5c890-p101">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below. For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="5c890-105">在 Windows 搜尋] 方塊中，輸入執行，請選取 [執行桌面應用程式、 類型 services.msc 與然後選取 [ **Enter**。</span><span class="sxs-lookup"><span data-stu-id="5c890-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="5c890-p102">捲動到 WebClient 服務，並檢查 [**狀態**] 欄。如果 WebClient 服務狀態不**執行**，連按兩下 [服務、 按一下 [**開始**] 及 [**確定]**。必要時，在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**啟用服務]。</span><span class="sxs-lookup"><span data-stu-id="5c890-p102">Scroll down to the WebClient service and check the **Status** column. If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**. Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5c890-p103">若要疑難排解在檔案總管] 中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。探索更好的替代項為同步處理：[同步處理 SharePoint 檔案與新 OneDrive sync 用戶端](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="5c890-p103">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665). Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

