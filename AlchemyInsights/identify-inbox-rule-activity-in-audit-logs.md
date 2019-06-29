---
title: 在審計記錄檔中識別收件匣規則活動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 51c25897223371a6dcc94c948955107ce74b0e8e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383016"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="44b9d-102">在審計記錄檔中識別收件匣規則活動</span><span class="sxs-lookup"><span data-stu-id="44b9d-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="44b9d-103">您可以使用安全性 & 合規性中心內的審核記錄搜尋, 來查看收件匣規則事件 (建立、修改及刪除收件匣規則)。</span><span class="sxs-lookup"><span data-stu-id="44b9d-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="44b9d-104">登入[Office 365 安全性 & 規範中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="44b9d-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="44b9d-105">按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="44b9d-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="44b9d-106">選取 [**開始日期**] 和 [**結束日期**] 欄位中的日期範圍。</span><span class="sxs-lookup"><span data-stu-id="44b9d-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="44b9d-107">在 [ **Exchange 信箱活動**] 下, 確認 [**活動**] 欄位已設定為 [ **disable-inboxrule 程式建立/修改/啟用/停用收件匣規則**]。</span><span class="sxs-lookup"><span data-stu-id="44b9d-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="44b9d-108">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="44b9d-108">Click **Search**.</span></span>

<span data-ttu-id="44b9d-109">在結果中, 選取一筆審計記錄。</span><span class="sxs-lookup"><span data-stu-id="44b9d-109">In the results, select an audit record.</span></span> <span data-ttu-id="44b9d-110">在 [詳細資料] 快顯視窗中, 按一下 [**詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="44b9d-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="44b9d-111">收件匣規則設定的相關資訊會顯示在 [**參數**] 欄位中。</span><span class="sxs-lookup"><span data-stu-id="44b9d-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="44b9d-112">如需詳細資訊, 請參閱[決定使用者建立的收件匣規則](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="44b9d-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
