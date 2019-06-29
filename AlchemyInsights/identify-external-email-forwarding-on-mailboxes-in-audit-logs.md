---
title: 在審計記錄檔中識別信箱上的外部電子郵件轉寄
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 43b6a26bc05892e71d41c4b47522785245cb4851
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35383088"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="f5c2c-102">識別信箱上設定外部電子郵件轉寄的時機</span><span class="sxs-lookup"><span data-stu-id="f5c2c-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="f5c2c-103">當使用者在信箱上設定外部電子郵件轉寄時, 會將活動作為**設定信箱指令程式**的一部分進行審核。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-103">When a user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="f5c2c-104">您可以在安全性 & 規範中心內使用 [審核記錄搜尋] 來查看活動。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="f5c2c-105">登入[Office 365 安全性 & 規範中心](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f5c2c-105">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="f5c2c-106">按一下 [**搜尋和調查**], 然後選取 [**審核記錄搜尋**]。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-106">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="f5c2c-107">選取 [**開始日期**] 和 [**結束日期**] 欄位中的日期範圍。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f5c2c-108">您不需要指定使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-108">You don't need to specify a username.</span></span> <span data-ttu-id="f5c2c-109">確認 [**活動**] 欄位已設為 [**顯示所有活動的結果**]。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="f5c2c-110">Click **Search**.</span><span class="sxs-lookup"><span data-stu-id="f5c2c-110">Click **Search**.</span></span>

<span data-ttu-id="f5c2c-111">在結果中, 按一下 [**篩選結果**], 然後在 [活動篩選] 方塊中輸入**集-信箱**。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="f5c2c-112">在結果中選取一筆審計記錄。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-112">Select an audit record in the results.</span></span> <span data-ttu-id="f5c2c-113">在 [**詳細資料**] 快顯視窗中, 按一下 [**詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="f5c2c-114">您必須查看每個審計記錄的詳細資料, 以判斷活動是否與電子郵件轉寄有關。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="f5c2c-115">**ObjectId**: 已修改之信箱的別名值。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="f5c2c-116">**參數**: _ForwardingSmtpAddress_指出目標電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="f5c2c-117">**UserId**: 在 [ **ObjectId** ] 欄位的信箱上設定電子郵件轉寄的使用者。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="f5c2c-118">如需詳細資訊, 請參閱[決定如何設定信箱的電子郵件](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。</span><span class="sxs-lookup"><span data-stu-id="f5c2c-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).</span></span>
