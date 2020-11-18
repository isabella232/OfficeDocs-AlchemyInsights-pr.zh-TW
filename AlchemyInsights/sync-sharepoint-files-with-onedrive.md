---
title: 疑難排解 Sharepoint Online 中的「 在檔案總管中開啟」問題
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6462"
- "9003546"
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ea93bb6f3cbbc3424f5e006ffac482a7445c8164
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086039"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="4a68e-102">疑難排解 Sharepoint Online 中的「 在檔案總管中開啟」問題</span><span class="sxs-lookup"><span data-stu-id="4a68e-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="4a68e-103">請遵循下列文章中的步驟和最佳做法進行：</span><span class="sxs-lookup"><span data-stu-id="4a68e-103">Follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="4a68e-104">[如何使用 [在檔案總管中開啟] 命令以在 SharePoint Online 中針對問題進行疑難排解](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span><span class="sxs-lookup"><span data-stu-id="4a68e-104">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/troubleshoot/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span></span>

- <span data-ttu-id="4a68e-105">[使用 [在檔案總管中開啟] 來複製或移動檔案](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)</span><span class="sxs-lookup"><span data-stu-id="4a68e-105">[Copy or move library files by using Open with Explorer](https://support.microsoft.com/office/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2?ui=en-us&rs=en-us&ad=us)</span></span>

> [!NOTE]
- <span data-ttu-id="4a68e-106">建議您[將 SharePoint 檔案與新版 [OneDrive 同步處理用戶端] 同步](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us)，其提供 [檔案隨選](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us)，因為同步處理可讓您在本機存取您的檔案，並提供最佳效能。</span><span class="sxs-lookup"><span data-stu-id="4a68e-106">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88?ui=en-us&rs=en-us&ad=us) which provides [Files On-Demand](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-us&rs=en-us&ad=us) because the synchronization grants local access to your files and offers the best performance.</span></span>

- <span data-ttu-id="4a68e-107">只有 Internet Explorer 11 支援 **[在檔案總管中開啟]**。</span><span class="sxs-lookup"><span data-stu-id="4a68e-107">**Open with Explorer** is only supported in Internet Explorer 11.</span></span> <span data-ttu-id="4a68e-108">如需詳細資訊，請參閱 [終止對 IE11 與[Microsoft 365 Apps] 的支援服務 ](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy))。</span><span class="sxs-lookup"><span data-stu-id="4a68e-108">For more information, see [end of support for IE11 with Microsoft 365 Apps](https://docs.microsoft.com/lifecycle/announcements/m365-ie11-microsoft-edge-legacy)).</span></span> <span data-ttu-id="4a68e-109">**[在檔案總管中開啟]** 無法用於 Windows 的 Microsoft Edge、Google Chrome、Mozilla Firefox，或 Mac 平台上。</span><span class="sxs-lookup"><span data-stu-id="4a68e-109">**Open with Explorer** doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="4a68e-110">因為這個原因，**[總管檢視]** 選項可能會呈現灰色。</span><span class="sxs-lookup"><span data-stu-id="4a68e-110">Due to this reason, the **Explorer View** option may be grayed out.</span></span> 

- <span data-ttu-id="4a68e-111">新版文件庫不會顯示 **[在檔案總管中開啟]** 按鈕。</span><span class="sxs-lookup"><span data-stu-id="4a68e-111">The **Open with Explorer** button doesn't appear in the new library experience.</span></span> <span data-ttu-id="4a68e-112">選取右上方的 **[檢視]** 下拉式清單 (下拉式清單的名稱依您的檢視畫面而定)，再選取 **[在 [檔案總管] 中檢視]**。</span><span class="sxs-lookup"><span data-stu-id="4a68e-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>

