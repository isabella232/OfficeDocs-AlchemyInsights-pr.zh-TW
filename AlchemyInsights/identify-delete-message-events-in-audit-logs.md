---
title: 識別刪除稽核記錄中的郵件事件
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909081"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="89780-102">稽核記錄檔的已刪除的電子郵件訊息</span><span class="sxs-lookup"><span data-stu-id="89780-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="89780-103">2019 年 1 月開始，信箱稽核記錄預設會開啟 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="89780-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="89780-104">否則，若要檢閱刪除特定使用者的郵件事件，您需要以手動啟用稽核的刪除動作。</span><span class="sxs-lookup"><span data-stu-id="89780-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="89780-105">如果信箱稽核記錄已啟用您的組織或特定使用者，請遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="89780-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="89780-106">登入[Office 365 安全性 & 合規性中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="89780-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="89780-107">按一下 [**搜尋和調查**，然後選取 [**稽核記錄搜尋**。</span><span class="sxs-lookup"><span data-stu-id="89780-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="89780-108">在 [**開始日期**和**結束日期**] 欄位中選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="89780-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="89780-109">指定您想要調查 （使用者刪除的項目） 的使用者的使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="89780-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="89780-110">在 [**活動**] 欄位中，選取 [**刪除的項目資料夾中的已刪除郵件**和**Moved 郵件提交至刪除的項目] 資料夾**。</span><span class="sxs-lookup"><span data-stu-id="89780-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="89780-111">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="89780-111">Click **Search**.</span></span>

<span data-ttu-id="89780-112">在結果中，選取 [稽核記錄]。</span><span class="sxs-lookup"><span data-stu-id="89780-112">In the results, select an audit record.</span></span> <span data-ttu-id="89780-113">在詳細資料彈出式視窗中，按一下 [**更多的資訊**。</span><span class="sxs-lookup"><span data-stu-id="89780-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="89780-114">已刪除的項目 （例如，[主旨] 行和時已刪除之項目的位置） 的其他資訊會顯示在 [ **AffectedItems** ] 欄位。</span><span class="sxs-lookup"><span data-stu-id="89780-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="89780-115">**ClientInfoString**屬性將會顯示在 Outlook 中，Outlook （先前稱為 Outlook Web App） 或任何其他裝置上是否發生刪除。</span><span class="sxs-lookup"><span data-stu-id="89780-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="89780-116">如需詳細資訊，請參閱 <<c0>的判斷設定電子郵件轉寄的信箱。</span><span class="sxs-lookup"><span data-stu-id="89780-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="89780-117">**附註**： 您無法擷取已刪除的項目使用的稽核記錄功能。</span><span class="sxs-lookup"><span data-stu-id="89780-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="89780-118">若要擷取網頁型 Outlook 中已刪除的郵件，請參閱[復原已刪除的 Outlook Web App 中的項目](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)。</span><span class="sxs-lookup"><span data-stu-id="89780-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
