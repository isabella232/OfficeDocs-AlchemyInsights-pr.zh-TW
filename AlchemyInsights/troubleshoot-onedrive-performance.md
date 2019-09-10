---
title: 疑難排解 OneDrive 效能
ms.author: pebaum
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 222f818c3fd78a19b9952d4703755498bc080910
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822189"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="5703a-102">疑難排解 OneDrive 效能</span><span class="sxs-lookup"><span data-stu-id="5703a-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="5703a-103">如果您遇到速度較慢比預期的同步處理或與 OneDrive 類似的效能問題：</span><span class="sxs-lookup"><span data-stu-id="5703a-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="5703a-104">請確認沒有任何使用[服務健全狀況儀表板](https://portal.office.com/adminportal/home?ref=/servicehealth)的已知的問題。</span><span class="sxs-lookup"><span data-stu-id="5703a-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="5703a-105">[啟用隨選檔案](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US)，讓您可以存取您在 OneDrive 中的所有檔案，而不需下載全部，然後使用您的裝置上的儲存空間。</span><span class="sxs-lookup"><span data-stu-id="5703a-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e?ui=en-US&rs=en-US&ad=US) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="5703a-106">網路規劃和效能[檢閱的最佳作法](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)。</span><span class="sxs-lookup"><span data-stu-id="5703a-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="5703a-107">[上傳與下載速度最大化](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)，尤其是如果您第一次同步處理的裝置。</span><span class="sxs-lookup"><span data-stu-id="5703a-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="5703a-108">如果您正在同步處理超過 100000 個項目與文件庫，OneDrive 同步處理似乎停滯很長的時間，或 [狀態] 顯示處理的 xMB 0 KB。 」</span><span class="sxs-lookup"><span data-stu-id="5703a-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="5703a-109">[了解更多關於同步處理超過 100000 檔案](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)，以及[300000 檔案的 OneDrive 的支援的限制](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)。</span><span class="sxs-lookup"><span data-stu-id="5703a-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="5703a-110">當使用者超過使用量限制時，SharePoint Online 節流處理任何進一步的要求，從該使用者帳戶在短期間內。</span><span class="sxs-lookup"><span data-stu-id="5703a-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="5703a-111">節流生效時，會受到節流的所有使用者動作。</span><span class="sxs-lookup"><span data-stu-id="5703a-111">All user actions are throttled while the throttle is in effect.</span></span>
