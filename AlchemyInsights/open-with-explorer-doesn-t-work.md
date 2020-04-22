---
title: 使用 Explorer 開啟無法運作
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: dc939a3451ff4fe95e4aa5a999839a2c532b398c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713025"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="c4f6d-102">使用 Explorer 開啟無法運作</span><span class="sxs-lookup"><span data-stu-id="c4f6d-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="c4f6d-103">[**開啟時使用 Explorer** ] 或 [檔案**瀏覽器中的視圖**無法運作請遵循下列**步驟，確定**WebClient 服務已設定為執行]。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="c4f6d-104">例如，當服務未執行時，可能需要很長的時間才能開啟 SharePoint 或 OneDrive 文件庫。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="c4f6d-105">在 [Windows 搜尋] 方塊中，輸入 run，選取 [執行桌面應用程式]，輸入 services.msc，然後選取**Enter**。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="c4f6d-106">向左下到 WebClient 服務，然後查看 [**狀態**] 欄。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="c4f6d-107">如果 WebClient 服務**狀態未執行，請**按兩下服務，按一下 [**開始**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="c4f6d-108">如有需要，請在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**]，以啟用服務。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="c4f6d-109">若要疑難排解在檔案瀏覽器中開啟的問題，請參閱[在瀏覽器中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="c4f6d-110">探索同步[處理：使用新的 OneDrive 同步處理用戶端來同步處理 SharePoint](https://go.microsoft.com/fwlink/?linkid=871666)檔案。</span><span class="sxs-lookup"><span data-stu-id="c4f6d-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

