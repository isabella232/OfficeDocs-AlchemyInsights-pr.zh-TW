---
title: 疑難排解 OneDrive 效能
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 197a84c5f69f9e58460925049345263743fe78ee
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43733189"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="21f4e-102">疑難排解 OneDrive 效能</span><span class="sxs-lookup"><span data-stu-id="21f4e-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="21f4e-103">如果您的同步處理速度慢，或 OneDrive 發生類似效能問題：</span><span class="sxs-lookup"><span data-stu-id="21f4e-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="21f4e-104">確認使用[服務健康情況儀表板](https://portal.office.com/adminportal/home?ref=/servicehealth)沒有已知問題。</span><span class="sxs-lookup"><span data-stu-id="21f4e-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="21f4e-105">[根據需要啟用](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)檔案，讓您可以在 OneDrive 中存取所有檔案，而不必下載所有檔案，並在裝置上使用儲存空間。</span><span class="sxs-lookup"><span data-stu-id="21f4e-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="21f4e-106">查看網路規劃和效能的[最佳作法](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance)。</span><span class="sxs-lookup"><span data-stu-id="21f4e-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="21f4e-107">[最大化上傳與下載速度](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43)，尤其是在您第一次同步處理裝置時。</span><span class="sxs-lookup"><span data-stu-id="21f4e-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="21f4e-108">如果您同步處理的文件庫具有超過100000個專案，OneDrive 同步處理可能會在很長的時間停滯，否則狀態會顯示 xMB 的 [處理 0KB]。</span><span class="sxs-lookup"><span data-stu-id="21f4e-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="21f4e-109">[深入瞭解如何同步處理超過100000個](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)檔案，以及[OneDrive 支援的300000檔限制](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa)。</span><span class="sxs-lookup"><span data-stu-id="21f4e-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="21f4e-110">當使用者超過使用限制時，SharePoint 線上會在短期內限制來自該使用者帳戶的任何要求。</span><span class="sxs-lookup"><span data-stu-id="21f4e-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="21f4e-111">節流生效時，所有的使用者動作都會遭到節流。</span><span class="sxs-lookup"><span data-stu-id="21f4e-111">All user actions are throttled while the throttle is in effect.</span></span>
