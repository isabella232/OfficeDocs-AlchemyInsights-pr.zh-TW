---
title: 未傳遞 SharePoint 警示通知
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742038"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="08d5f-102">未傳遞 SharePoint 警示通知</span><span class="sxs-lookup"><span data-stu-id="08d5f-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="08d5f-103">請檢查您電子郵件中的 [垃圾郵件] 資料夾，因為有時候提醒可能會到達這裡。</span><span class="sxs-lookup"><span data-stu-id="08d5f-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="08d5f-104">決定是否**未傳遞所有警示**，或是未傳遞特定檔案或文件庫中**的個別警示**。</span><span class="sxs-lookup"><span data-stu-id="08d5f-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="08d5f-105">**未傳遞個別警示**：如果未傳遞特定檔案或文件庫中的個別警示，您可以嘗試刪除並重新建立。</span><span class="sxs-lookup"><span data-stu-id="08d5f-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="08d5f-106">請參閱[管理、查看或刪除 SharePoint 警示](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)，以重新建立警示。</span><span class="sxs-lookup"><span data-stu-id="08d5f-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="08d5f-107">**未傳遞所有警示**：如果未傳遞所有來自多個檔案或文件庫的警示，請造訪[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，檢查是否有任何 SharePoint 或 Exchange 可能發生的諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="08d5f-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="08d5f-108">問題可能是透過 Exchange 在電子郵件中 SharePoint 警示功能或延遲。</span><span class="sxs-lookup"><span data-stu-id="08d5f-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="08d5f-109">此外，請務必注意是否正在傳遞其他電子郵件，如果不是，則可能是 Exchange 延遲的問題。</span><span class="sxs-lookup"><span data-stu-id="08d5f-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="08d5f-110">警示上的常見問題：</span><span class="sxs-lookup"><span data-stu-id="08d5f-110">FAQ on alerts:</span></span>

- <span data-ttu-id="08d5f-111">無法將提醒傳送給通訊群組，只支援 Security 和 O365 群組。</span><span class="sxs-lookup"><span data-stu-id="08d5f-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="08d5f-112">您無法自訂警示電子郵件範本;您必須使用 Microsoft FLOW 或 SharePoint Designer 工作流程來達成這類工作流程。</span><span class="sxs-lookup"><span data-stu-id="08d5f-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

<span data-ttu-id="08d5f-113">詳細資訊：</span><span class="sxs-lookup"><span data-stu-id="08d5f-113">More Information:</span></span>

- <span data-ttu-id="08d5f-114">**警示設定**：如需有關設定警示的詳細資訊，請參閱[建立警示，以在 SharePoint 中的檔案或資料夾變更時取得通知](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)。</span><span class="sxs-lookup"><span data-stu-id="08d5f-114">**Alert setup**: For more information about setting up alerts, see [Create an alert to get notified when a file or folder changes in SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).</span></span>
- <span data-ttu-id="08d5f-115">**警示疑難排解**：如需疑難排解提醒的詳細資訊，請參閱[使用者不會收到 SharePoint 線上警示通知](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)。</span><span class="sxs-lookup"><span data-stu-id="08d5f-115">**Troubleshoot alerts**: For more information about troubleshooting alerts, see [Users don't receive SharePoint Online alert notifications](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).</span></span>
- <span data-ttu-id="08d5f-116">**高級 O365 相容性警示原則**：如需設定這些警示的詳細資訊，請參閱[相容性警示原則](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。</span><span class="sxs-lookup"><span data-stu-id="08d5f-116">**Advanced O365 Compliance Alert Policies**: For more information about setting up these alerts, see [Compliance Alert Policies](https://docs.microsoft.com/office365/securitycompliance/alert-policies).</span></span>
- <span data-ttu-id="08d5f-117">**SharePoint 和 OneDrive 審核記錄**檔：如需如何取得這些事件的詳細資訊，請參閱[搜尋審核記錄](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)檔。</span><span class="sxs-lookup"><span data-stu-id="08d5f-117">**SharePoint and OneDrive Audit Logs**: For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
- <span data-ttu-id="08d5f-118">**由「高級威脅防護」所傳送的警示**：請參閱[SharePoint 和 OneDrive 的 ATP](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="08d5f-118">**Alerts sent by Advanced Threat Protection**: See [ATP for SharePoint and OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
- <span data-ttu-id="08d5f-119">**資料遺失防護原則所傳送的警示**：請參閱[DLP 原則的電子郵件通知](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)。</span><span class="sxs-lookup"><span data-stu-id="08d5f-119">**Alerts sent by Data Loss Prevention polices**: See [Email notifications for DLP policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

## <a name="related-topics"></a><span data-ttu-id="08d5f-120">相關主題</span><span class="sxs-lookup"><span data-stu-id="08d5f-120">Related Topics</span></span>

<span data-ttu-id="08d5f-121">想要在 SharePoint Online 中試用 Microsoft 流程嗎？</span><span class="sxs-lookup"><span data-stu-id="08d5f-121">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="08d5f-122">建立流程</span><span class="sxs-lookup"><span data-stu-id="08d5f-122">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="08d5f-123">SharePoint 和流程</span><span class="sxs-lookup"><span data-stu-id="08d5f-123">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
