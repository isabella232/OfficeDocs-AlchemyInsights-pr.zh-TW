---
title: 在審計記錄檔中識別收件匣規則活動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f946510539b3d28f2ceeec1546cbffce8bd352fd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716415"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="4b1b1-102">在審計記錄檔中識別收件匣規則活動</span><span class="sxs-lookup"><span data-stu-id="4b1b1-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="4b1b1-103">您可以在 Microsoft 365 Security & 合規性中心內使用審核記錄搜尋，以查看收件匣規則事件（建立、修改及刪除收件匣規則）。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="4b1b1-104">登入[Microsoft 365 的安全性 & 規範中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="4b1b1-105">移至 [**搜尋** > **審核記錄搜尋**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="4b1b1-106">在 [**開始日期**] 和 [**結束日期**] 欄位中，選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="4b1b1-107">在 [ **Exchange 信箱活動**] 底下，確認 [**活動**] 欄位已設定為**New-InboxRule 建立/修改/啟用/停用收件匣規則**。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="4b1b1-108">按一下 [搜尋]。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-108">Click **Search**.</span></span>

<span data-ttu-id="4b1b1-109">在結果中，選取一個審計記錄。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-109">In the results, select an audit record.</span></span> <span data-ttu-id="4b1b1-110">在 [詳細資料] 快顯視窗中，按一下 [**詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="4b1b1-111">[**參數**] 欄位中會顯示 [收件匣規則] 設定的相關資訊。</span><span class="sxs-lookup"><span data-stu-id="4b1b1-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="4b1b1-112">如需詳細資訊，請參閱[判斷使用者是否建立收件匣規則](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="4b1b1-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
