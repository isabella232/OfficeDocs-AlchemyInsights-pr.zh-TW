---
title: 疑難排解 Sharepoint Online 中的「 在檔案總管中開啟」問題
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/7/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 73583b3b27143c708a4cc993cdff94a33131ab52
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/04/2019
ms.locfileid: "36743084"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="9a155-102">疑難排解 Sharepoint Online 中的「 在檔案總管中開啟」問題</span><span class="sxs-lookup"><span data-stu-id="9a155-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="9a155-103">[在檔案總管中開啟] 命令會開啟 [Windows 檔案總管] 的本機執行個體，並顯示主控 SharePoint 網站的伺服器上的資料夾結構。</span><span class="sxs-lookup"><span data-stu-id="9a155-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="9a155-104">因此，我們建議您[將 SharePoint 檔案與新的 OneDrive 同步處理用戶端同步](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>，其提供 [檔案隨選][](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)，因為它可讓您在本機存取您的檔案，並提供最佳效能。</span><span class="sxs-lookup"><span data-stu-id="9a155-104">This being said, we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="9a155-105">如果您選擇使用總管檢視，而非使用新的 OneDrive 同步用戶端，請務必遵循以下文章中提供的步驟及最佳做法：</span><span class="sxs-lookup"><span data-stu-id="9a155-105">If you chose to use Explorer view instead of using the new OneDrive sync client, make sure you follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="9a155-106">[如何使用 [在檔案總管中開啟] 命令以在 SharePoint Online 中針對問題進行疑難排解](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) (英文)</span><span class="sxs-lookup"><span data-stu-id="9a155-106">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span></span>

- <span data-ttu-id="9a155-107">[使用 [在檔案總管中開啟] 來複製或移動檔案](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2) (機器翻譯)</span><span class="sxs-lookup"><span data-stu-id="9a155-107">[Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span></span>

> [!Note]  
> <span data-ttu-id="9a155-108">新版文件庫不會顯示 [在檔案總管中開啟] \*\*\*\* 按鈕。</span><span class="sxs-lookup"><span data-stu-id="9a155-108">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="9a155-109">選取右上方的 [檢視]\*\*\*\* 下拉式清單 (下拉式清單的名稱依您的檢視畫面而定)，再選取 [在 [檔案總管] 中檢視]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="9a155-109">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
>
 ><span data-ttu-id="9a155-110">SharePoint 的 [在檔案總管中開啟] 使用 ActiveX 控制項，所以只支援 Internet Explorer 10 或 11。</span><span class="sxs-lookup"><span data-stu-id="9a155-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="9a155-111">[在檔案總管中開啟] 無法用於 Windows 的 Microsoft Edge、Google Chrome、Mozilla Firefox，或 Mac 平台上。</span><span class="sxs-lookup"><span data-stu-id="9a155-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="9a155-112">因為這個原因，[檔案總管檢視] 選項可能會呈現灰色。</span><span class="sxs-lookup"><span data-stu-id="9a155-112">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
> - <span data-ttu-id="9a155-113">[為什麼 SharePoint 功能區按鈕無法使用或呈現灰色](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca)。</span><span class="sxs-lookup"><span data-stu-id="9a155-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  

