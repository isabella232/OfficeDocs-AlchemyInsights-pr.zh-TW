---
title: 傳統 SharePoint 的審計記錄報告
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662199"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ff556-102">SharePoint 和 OneDrive 審核記錄檔</span><span class="sxs-lookup"><span data-stu-id="ff556-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ff556-103">SharePoint 傳統的審計記錄</span><span class="sxs-lookup"><span data-stu-id="ff556-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ff556-104">SPO 舊版審核已遷移至整合的審計記錄檔 (UAL) 。</span><span class="sxs-lookup"><span data-stu-id="ff556-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ff556-105">所有 SPO 的舊版審核報告現在都會透過 UAL 供電，舊版的審核信號也會遷移至 UAL。</span><span class="sxs-lookup"><span data-stu-id="ff556-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ff556-106">主要變更：</span><span class="sxs-lookup"><span data-stu-id="ff556-106">Key changes:</span></span>

* <span data-ttu-id="ff556-107">無法使用修整功能。</span><span class="sxs-lookup"><span data-stu-id="ff556-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ff556-108">無法使用選擇要進行審核的特定事件。</span><span class="sxs-lookup"><span data-stu-id="ff556-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ff556-109">請參閱 [本檔](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) ，以取得預設可供使用之審核事件的完整清單。</span><span class="sxs-lookup"><span data-stu-id="ff556-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ff556-110">無法使用 [**自訂報告**] 底下的 [**位置**] 選項。</span><span class="sxs-lookup"><span data-stu-id="ff556-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ff556-111">無法使用「 **開啟或下載檔案** 的事件] 選項。</span><span class="sxs-lookup"><span data-stu-id="ff556-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ff556-112">設定網站集合的審核設定</span><span class="sxs-lookup"><span data-stu-id="ff556-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ff556-113">從相容性中 SharePoint 和 OneDrive 現代化的整合審計記錄檔</span><span class="sxs-lookup"><span data-stu-id="ff556-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ff556-114">開啟/關閉整合的審計記錄</span><span class="sxs-lookup"><span data-stu-id="ff556-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ff556-115">SharePoint 或 OneDrive 中不需要進行其他設定。</span><span class="sxs-lookup"><span data-stu-id="ff556-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ff556-116">使用「審核記錄搜尋」檢查檔案 (s) 、資料夾 () 、使用者 () 、許可權的活動：</span><span class="sxs-lookup"><span data-stu-id="ff556-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ff556-117">檔案和頁面活動</span><span class="sxs-lookup"><span data-stu-id="ff556-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ff556-118">資料夾活動</span><span class="sxs-lookup"><span data-stu-id="ff556-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ff556-119">共用及存取要求活動</span><span class="sxs-lookup"><span data-stu-id="ff556-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ff556-120">同步處理活動</span><span class="sxs-lookup"><span data-stu-id="ff556-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ff556-121">網站管理活動</span><span class="sxs-lookup"><span data-stu-id="ff556-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ff556-122">如需如何取得這些事件的詳細資訊，請參閱 [搜尋審核記錄](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)檔。</span><span class="sxs-lookup"><span data-stu-id="ff556-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
