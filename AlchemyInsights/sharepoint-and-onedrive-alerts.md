---
title: 接收 SharePoint 和 OneDrive 提醒時的延遲
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785656"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="26610-102">接收 SharePoint 和 OneDrive 提醒時的延遲</span><span class="sxs-lookup"><span data-stu-id="26610-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="26610-103">先檢查您電子郵件中的 [垃圾郵件] 或 [垃圾郵件] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="26610-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="26610-104">若 **所有來自多個檔案或文件庫的警示都延遲**，請造訪 [服務健康情況儀表板](https://portal.office.com/adminportal/home?ref=/servicehealth) ，檢查是否有任何 SharePoint 或 Exchange 可能發生的諮詢/事件。</span><span class="sxs-lookup"><span data-stu-id="26610-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="26610-105">此問題可能是透過 Exchange 在電子郵件中使用 SharePoint 警示功能或延遲。</span><span class="sxs-lookup"><span data-stu-id="26610-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="26610-106">另外請注意，是否有傳送其他電子郵件; 如果不是，則問題可能是 Exchange 延遲。</span><span class="sxs-lookup"><span data-stu-id="26610-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="26610-107">如果 **未傳遞特定檔案或文件庫中的個別警示**，請嘗試刪除並重新建立。</span><span class="sxs-lookup"><span data-stu-id="26610-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="26610-108">請參閱 [管理、查看或刪除 SharePoint 警示](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) ，以重新建立警示。</span><span class="sxs-lookup"><span data-stu-id="26610-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="26610-109">無法將警示傳送至通訊群組。</span><span class="sxs-lookup"><span data-stu-id="26610-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="26610-110">只支援 Security 和 O365 群組。</span><span class="sxs-lookup"><span data-stu-id="26610-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="26610-111">您無法自訂警示電子郵件範本。</span><span class="sxs-lookup"><span data-stu-id="26610-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="26610-112">您必須使用 Microsoft 流程或 SharePoint 設計者工作流程來達成這些工作流程。</span><span class="sxs-lookup"><span data-stu-id="26610-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
