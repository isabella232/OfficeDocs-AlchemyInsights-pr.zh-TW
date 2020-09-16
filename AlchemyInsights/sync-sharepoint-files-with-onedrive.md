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
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: ba9f11da5c35c3681e9bd5ceaf13233fe8b80fc9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737296"
---
# <a name="troubleshoot-open-with-explorer-issues-in-sharepoint-online"></a><span data-ttu-id="e9a3c-102">疑難排解 Sharepoint Online 中的「 在檔案總管中開啟」問題</span><span class="sxs-lookup"><span data-stu-id="e9a3c-102">Troubleshoot “Open with Explorer” issues in SharePoint Online</span></span>

<span data-ttu-id="e9a3c-103">建議您[將 SharePoint 檔案與新的 OneDrive 同步處理用戶端同步](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)，其提供 [檔案隨選][](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e)，因為它可讓您在本機存取您的檔案，並提供最佳效能。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-103">We recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88) which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>

<span data-ttu-id="e9a3c-104">若要疑難排解 [在檔案總管中開啟] 的問題，請遵循下列文章中的步驟和最佳做法進行：</span><span class="sxs-lookup"><span data-stu-id="e9a3c-104">To troubleshoot Open with Explorer issues, follow the steps and best practices in the following articles:</span></span>

- <span data-ttu-id="e9a3c-105">[如何使用 [在檔案總管中開啟] 命令以在 SharePoint Online 中針對問題進行疑難排解](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) (英文)</span><span class="sxs-lookup"><span data-stu-id="e9a3c-105">[How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer)</span></span>
- <span data-ttu-id="e9a3c-106">[使用 [在檔案總管中開啟] 來複製或移動檔案](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span><span class="sxs-lookup"><span data-stu-id="e9a3c-106">[Copy or move library files by using Open with Explorer](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)</span></span>

> <span data-ttu-id="e9a3c-107">**附註：**</span><span class="sxs-lookup"><span data-stu-id="e9a3c-107">**Note:**</span></span>
>- <span data-ttu-id="e9a3c-108">只有 Internet Explorer 10 或 11 支援「在檔案總管中開啟」。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-108">Open with Explorer is only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="e9a3c-109">[在檔案總管中開啟] 無法用於 Windows 的 Microsoft Edge、Google Chrome、Mozilla Firefox，或 Mac 平台上。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-109">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="e9a3c-110">因為這個原因，[檔案總管檢視] 選項可能會呈現灰色。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-110">Due to this reason, the Explorer View option may be grayed out.</span></span>
>
>- <span data-ttu-id="e9a3c-111">新版文件庫不會顯示 [在檔案總管中開啟] 按鈕。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-111">The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="e9a3c-112">選取右上方的 **[檢視]** 下拉式清單 (下拉式清單的名稱依您的檢視畫面而定)，再選取 **[在 [檔案總管] 中檢視]**。</span><span class="sxs-lookup"><span data-stu-id="e9a3c-112">Select the **View** drop-down in the upper right (the name of the drop-down changes depending on your current view), and then select **View in File Explorer**.</span></span>
