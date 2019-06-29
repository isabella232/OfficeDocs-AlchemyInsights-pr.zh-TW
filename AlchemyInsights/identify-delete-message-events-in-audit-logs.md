---
title: 在審核記錄檔中識別刪除郵件事件
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 89877331d328d798177fab3150d5219c5b484a70
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383124"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="70047-102">已刪除電子郵件的審計記錄檔</span><span class="sxs-lookup"><span data-stu-id="70047-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="70047-103">從2019年1月開始, Microsoft 預設會開啟信箱審核記錄功能。</span><span class="sxs-lookup"><span data-stu-id="70047-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="70047-104">否則, 若要查看特定使用者的刪除郵件事件, 您必須手動啟用 [刪除] 動作以進行審核。</span><span class="sxs-lookup"><span data-stu-id="70047-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="70047-105">如果已為您的組織或特定使用者啟用信箱審核記錄, 請遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="70047-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="70047-106">登入[Office 365 安全性 & 規範中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="70047-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="70047-107">按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="70047-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="70047-108">選取 [**開始日期**] 和 [**結束日期**] 欄位中的日期範圍。</span><span class="sxs-lookup"><span data-stu-id="70047-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="70047-109">指定要調查之使用者的使用者名稱 (刪除專案的使用者)。</span><span class="sxs-lookup"><span data-stu-id="70047-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="70047-110">在 [**活動**] 欄位中, 選取 [**刪除的郵件] 資料夾中的 [刪除的郵件**], 並**將郵件移至 [刪除**</span><span class="sxs-lookup"><span data-stu-id="70047-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="70047-111">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="70047-111">Click **Search**.</span></span>

<span data-ttu-id="70047-112">在結果中, 選取一筆審計記錄。</span><span class="sxs-lookup"><span data-stu-id="70047-112">In the results, select an audit record.</span></span> <span data-ttu-id="70047-113">在 [詳細資料] 快顯視窗中, 按一下 [**詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="70047-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="70047-114">[ **AffectedItems** ] 欄位中會顯示已刪除專案的其他資訊 (例如, 當專案的主旨行和位置被刪除時)。</span><span class="sxs-lookup"><span data-stu-id="70047-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="70047-115">如果是在 Outlook、Outlook 網頁版 (先前稱為 Outlook Web App) 或任何其他裝置進行刪除, 則**ClientInfoString**屬性會顯示。</span><span class="sxs-lookup"><span data-stu-id="70047-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="70047-116">如需詳細資訊, 請參閱[決定如何設定信箱的電子郵件](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items)轉寄功能。</span><span class="sxs-lookup"><span data-stu-id="70047-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="70047-117">**附注**: 您無法使用 [audit log] 功能來取得已刪除的專案。</span><span class="sxs-lookup"><span data-stu-id="70047-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="70047-118">若要在 Outlook 網頁版中取得已刪除的郵件, 請參閱[在 Outlook Web App 中復原刪除的](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)郵件。</span><span class="sxs-lookup"><span data-stu-id="70047-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
