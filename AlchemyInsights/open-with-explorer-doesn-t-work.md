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
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30764899"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="8e61b-102">檔案總管中的開啟無法正常運作</span><span class="sxs-lookup"><span data-stu-id="8e61b-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="8e61b-103">如果**開啟檔案總管**] 或 [**在檔案總管中的檢視**無法確定 WebClient 服務會設定為**執行**下列步驟。</span><span class="sxs-lookup"><span data-stu-id="8e61b-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="8e61b-104">例如，可能需要很長的時間，若要開啟的 SharePoint 或 OneDrive 文件庫，當服務未執行。</span><span class="sxs-lookup"><span data-stu-id="8e61b-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="8e61b-105">在 [Windows 搜尋方塊中，輸入執行，請選取 [執行桌面應用程式類型 services.msc，然後選取 [**輸入**]。</span><span class="sxs-lookup"><span data-stu-id="8e61b-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="8e61b-106">捲動至 WebClient 服務，並檢查 [**狀態**] 欄。</span><span class="sxs-lookup"><span data-stu-id="8e61b-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="8e61b-107">如果 WebClient 服務狀態不**執行**，按兩下 [服務] 按一下 [**開始**]，然後按一下 [**確定]**。</span><span class="sxs-lookup"><span data-stu-id="8e61b-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="8e61b-108">如有需要選取 [**啟動類型**] 方塊中的 [**手動**] 或 [**自動**啟用 service]。</span><span class="sxs-lookup"><span data-stu-id="8e61b-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="8e61b-109">若要疑難排解在檔案總管中開啟的問題，請參閱[在檔案總管中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。</span><span class="sxs-lookup"><span data-stu-id="8e61b-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="8e61b-110">瀏覽更好的另一種方法的同步處理：[同步處理 SharePoint 檔案與新的 OneDrive 同步處理用戶端](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="8e61b-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

