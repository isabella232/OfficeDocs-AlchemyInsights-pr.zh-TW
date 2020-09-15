---
title: 在審計記錄檔中識別刪除郵件事件
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696504"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="6615f-102">已刪除電子郵件的審計記錄</span><span class="sxs-lookup"><span data-stu-id="6615f-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="6615f-103">從2019年1月開始，Microsoft 預設會開啟信箱審核記錄。</span><span class="sxs-lookup"><span data-stu-id="6615f-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="6615f-104">否則，若要查看特定使用者的刪除郵件事件，您必須手動啟用審核的刪除動作。</span><span class="sxs-lookup"><span data-stu-id="6615f-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="6615f-105">如果已為您的組織或特定使用者啟用信箱審核記錄，請遵循下列步驟。</span><span class="sxs-lookup"><span data-stu-id="6615f-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="6615f-106">登入 [Microsoft 365 的安全性 & 規範中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="6615f-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="6615f-107">按一下 [ **搜尋和調查** ]，然後選取 [ **審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="6615f-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="6615f-108">在 [ **開始日期** ] 和 [ **結束日期** ] 欄位中，選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="6615f-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="6615f-109">指定您要調查之使用者的使用者名稱)  (刪除專案的使用者。</span><span class="sxs-lookup"><span data-stu-id="6615f-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="6615f-110">在 [**活動**] 欄位中，選取 [**刪除的郵件] 資料夾中已刪除的郵件**，並**將郵件移至 [刪除的郵件**</span><span class="sxs-lookup"><span data-stu-id="6615f-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="6615f-111">按一下 [搜尋]。</span><span class="sxs-lookup"><span data-stu-id="6615f-111">Click **Search**.</span></span>

<span data-ttu-id="6615f-112">在結果中，選取一個審計記錄。</span><span class="sxs-lookup"><span data-stu-id="6615f-112">In the results, select an audit record.</span></span> <span data-ttu-id="6615f-113">在 [詳細資料] 快顯視窗中，按一下 [ **詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="6615f-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="6615f-114">已刪除專案的其他資訊 (例如，刪除專案的主旨行和位置) 會顯示在 [ **AffectedItems** ] 欄位中。</span><span class="sxs-lookup"><span data-stu-id="6615f-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="6615f-115">**ClientInfoString**屬性會顯示是否在 Outlook 中進行刪除，outlook 網頁版 outlook (之前稱為 Outlook web App) 或任何其他裝置。</span><span class="sxs-lookup"><span data-stu-id="6615f-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="6615f-116">如需詳細資訊，請參閱 [決定誰設定信箱的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)轉寄功能。</span><span class="sxs-lookup"><span data-stu-id="6615f-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="6615f-117">**附注**：您無法使用「審核記錄」功能來取得刪除的專案。</span><span class="sxs-lookup"><span data-stu-id="6615f-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="6615f-118">若要在 Outlook 網頁版中取得已刪除的郵件，請參閱 [在 Outlook Web App 中復原已刪除的](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)郵件。</span><span class="sxs-lookup"><span data-stu-id="6615f-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
