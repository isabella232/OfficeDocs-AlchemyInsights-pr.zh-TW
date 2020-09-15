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
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659049"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="2a4cf-102">修正使用 Explorer 開啟的問題</span><span class="sxs-lookup"><span data-stu-id="2a4cf-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="2a4cf-103">修正使用 [ **使用 [使用 [開啟] 瀏覽器** 命令在 SharePoint 或 OneDrive 中開啟文件庫時發生的常見問題：</span><span class="sxs-lookup"><span data-stu-id="2a4cf-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="2a4cf-104">使用 Internet Explorer 10 或 Internet Explorer 11。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="2a4cf-105">**使用 Explorer 開啟** 與 Microsoft Edge、Google Chrome、Firefox 及其他使用者不相容。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a4cf-106">在 Internet Explorer 以外的所有瀏覽器中停**用 Explorer 開啟**。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a4cf-107">在 SharePoint 文件庫的現代體驗中，無法使用**Explorer 開啟**。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="2a4cf-108">請改 **為在檔案資源管理器中使用 View** 。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="2a4cf-109">選取**View options**檔案 \> **瀏覽器中的**[view options view]。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="2a4cf-110">檔案瀏覽器中的視圖與 Microsoft Edge、Google Chrome、Firefox 及其他使用者不相容。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="2a4cf-111">僅能在 Internet Explorer 中**查看檔案資源管理器**中的。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="2a4cf-112">請確定 WebClient 服務正在執行中。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="2a4cf-113">在 [Windows 搜尋] 方塊中，輸入 run，選取 [執行桌面應用程式]，輸入 services.msc，然後按 Enter。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="2a4cf-114">向中向左下到 WebClient 服務，確定 [ **狀態** ] 欄顯示 "執行]。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="2a4cf-115">如果不是，請按兩下服務，按一下 [ **開始**]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="2a4cf-116"> (您可能需要先在 [**啟動類型**] 方塊中選取 [**手動**] 或 [**自動**]，以啟用服務。 ) </span><span class="sxs-lookup"><span data-stu-id="2a4cf-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="2a4cf-117">如果您只需要複製或移動多個檔案和資料夾一次，但是如果您想要在文件庫中經常運作，建議您將程式庫在檔案瀏覽器中開啟。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="2a4cf-118">若要疑難排解在檔案瀏覽器中開啟的問題，請參閱 [在瀏覽器中開啟](https://go.microsoft.com/fwlink/?linkid=871665)。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="2a4cf-119">如需設定同步處理的詳細資訊，請參閱 [sync SharePoint files with new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666)。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="2a4cf-120">如需詳細資訊，請參閱 [如何使用「開啟 With Explorer」命令來疑難排解 SharePoint Online 中的問題](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) 。</span><span class="sxs-lookup"><span data-stu-id="2a4cf-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

