---
title: 在審核記錄檔中識別 IP 位址和用戶端
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: a91778c006531371b85116f5c97485d42e6cc5be
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382944"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="1fa39-102">在審核記錄檔中識別 IP 位址和用戶端</span><span class="sxs-lookup"><span data-stu-id="1fa39-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="1fa39-103">對應至使用者或系統管理員活動的 IP 位址會顯示在 [Audit 記錄檔] 中。</span><span class="sxs-lookup"><span data-stu-id="1fa39-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="1fa39-104">也會記錄用戶端資訊。</span><span class="sxs-lookup"><span data-stu-id="1fa39-104">The client information is also logged.</span></span> <span data-ttu-id="1fa39-105">以下是識別此類資訊的步驟</span><span class="sxs-lookup"><span data-stu-id="1fa39-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="1fa39-106">登入[Office 365 安全性 & 規範中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="1fa39-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="1fa39-107">按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="1fa39-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="1fa39-108">如果您對特定活動感興趣, 請從 [**活動**] 清單中選取。</span><span class="sxs-lookup"><span data-stu-id="1fa39-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="1fa39-109">如果不是, 則會傳回所選使用者的所有活動 (預設設定)。</span><span class="sxs-lookup"><span data-stu-id="1fa39-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="1fa39-110">**附注**: 某些活動可能無法在 [**活動**] 功能表中使用;不過, 如果選取 [**顯示所有活動的結果**] (預設設定), 則會傳回這些審計專案。</span><span class="sxs-lookup"><span data-stu-id="1fa39-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="1fa39-111">在 [使用者] 欄位中指定**使用者**名稱, 為活動選取適當的日期範圍, 然後按一下 [**搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="1fa39-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="1fa39-112">在結果中, 您可以在 [結果] 窗格中看到該活動的 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="1fa39-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="1fa39-113">選取 [審核記錄], 以查看**詳細資料**快顯視窗中的詳細資訊 (例如, 用戶端、執行動作的使用者等等)。</span><span class="sxs-lookup"><span data-stu-id="1fa39-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="1fa39-114">如需詳細資訊, 請參閱[尋找用來存取已遭破壞之帳戶之電腦的 IP 位址](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。</span><span class="sxs-lookup"><span data-stu-id="1fa39-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
