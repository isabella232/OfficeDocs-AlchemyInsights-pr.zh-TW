---
title: 識別稽核記錄中的收件匣規則活動
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909082"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="b55c8-102">識別稽核記錄中的收件匣規則活動</span><span class="sxs-lookup"><span data-stu-id="b55c8-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="b55c8-103">您可以使用安全性 & 合規性中心中的稽核記錄搜尋，以檢視收件匣規則事件 （建立、 修改及刪除收件匣規則）。</span><span class="sxs-lookup"><span data-stu-id="b55c8-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="b55c8-104">登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="b55c8-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="b55c8-105">按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。</span><span class="sxs-lookup"><span data-stu-id="b55c8-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="b55c8-106">在 [**開始日期**和**結束日期**] 欄位中選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="b55c8-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="b55c8-107">在 [ **Exchange 信箱活動**，確認 [**活動**] 欄位設為**New-inboxrule 建立/修改/啟用/停用收件匣規則**。</span><span class="sxs-lookup"><span data-stu-id="b55c8-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="b55c8-108">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="b55c8-108">Click **Search**.</span></span>

<span data-ttu-id="b55c8-109">在結果中，選取 [稽核記錄]。</span><span class="sxs-lookup"><span data-stu-id="b55c8-109">In the results, select an audit record.</span></span> <span data-ttu-id="b55c8-110">在詳細資料彈出式視窗中，按一下 [**更多的資訊**。</span><span class="sxs-lookup"><span data-stu-id="b55c8-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="b55c8-111">在 [**參數**] 欄位會顯示收件匣規則設定相關資訊。</span><span class="sxs-lookup"><span data-stu-id="b55c8-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="b55c8-112">如需詳細資訊，請參閱 <<c0>判斷如果使用者所建立的收件匣規則</span><span class="sxs-lookup"><span data-stu-id="b55c8-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
