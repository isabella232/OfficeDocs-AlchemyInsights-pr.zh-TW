---
title: 識別 IP 位址和稽核記錄中的用戶端
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32416927"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="238bb-102">識別 IP 位址和稽核記錄中的用戶端</span><span class="sxs-lookup"><span data-stu-id="238bb-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="238bb-103">會對應至使用者或系統管理員活動的 IP 位址會顯示在稽核記錄檔。</span><span class="sxs-lookup"><span data-stu-id="238bb-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="238bb-104">用戶端資訊也會記錄。</span><span class="sxs-lookup"><span data-stu-id="238bb-104">The client information is also logged.</span></span> <span data-ttu-id="238bb-105">以下是用於識別此類資訊的步驟</span><span class="sxs-lookup"><span data-stu-id="238bb-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="238bb-106">登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="238bb-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="238bb-107">按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。</span><span class="sxs-lookup"><span data-stu-id="238bb-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="238bb-108">如果您有興趣的特定活動，請從**活動**清單中選取。</span><span class="sxs-lookup"><span data-stu-id="238bb-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="238bb-109">如果沒有，所選的使用者 （預設值） 會傳回所有活動。</span><span class="sxs-lookup"><span data-stu-id="238bb-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="238bb-110">**附註**： 某些活動可能無法在 [**活動**] 功能表中;不過，這些稽核項目將會傳回**所有活動顯示結果**是否已選取 （預設值）。</span><span class="sxs-lookup"><span data-stu-id="238bb-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="238bb-111">在 [**使用者**] 欄位中指定的使用者名稱，選取適當的日期範圍的活動，，然後按一下 [**搜尋**。</span><span class="sxs-lookup"><span data-stu-id="238bb-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="238bb-112">在結果中，您可以看到該活動在結果窗格中的 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="238bb-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="238bb-113">選取 [稽核記錄，以查看**詳細資料**彈出式視窗 （例如，用戶端，執行巨集指令、 等等的使用者。） 中的詳細的資訊。</span><span class="sxs-lookup"><span data-stu-id="238bb-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="238bb-114">如需詳細資訊，請參閱[尋找用來存取遭入侵的帳戶之電腦的 IP 位址](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)。</span><span class="sxs-lookup"><span data-stu-id="238bb-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
