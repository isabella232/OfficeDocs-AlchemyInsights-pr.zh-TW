---
title: 在審核記錄中識別信箱上的外部電子郵件轉發
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 592eb92e4b0fe0f9da2fa20bb93ffa4fbbb76662
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508943"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a><span data-ttu-id="72cc6-102">識別信箱上設定外部電子郵件轉寄的時間</span><span class="sxs-lookup"><span data-stu-id="72cc6-102">Identify when external email forwarding is configured on mailboxes</span></span>

<span data-ttu-id="72cc6-103">當 Microsoft 365 使用者設定信箱上的外部電子郵件轉寄功能時，會在**Set-Mailbox** Cmdlet 中審核該活動。</span><span class="sxs-lookup"><span data-stu-id="72cc6-103">When a Microsoft 365 user configures external email forwarding on a mailbox, the activity is audited as part of the **Set-Mailbox** cmdlet.</span></span> <span data-ttu-id="72cc6-104">您可以在安全性 & 規範中心內，看到使用審核記錄搜尋的活動。</span><span class="sxs-lookup"><span data-stu-id="72cc6-104">You can see the activity using audit log search in the Security & Compliance Center.</span></span>

1. <span data-ttu-id="72cc6-105">登入[Microsoft 365 的安全性 & 規範中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="72cc6-105">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="72cc6-106">移至 [**搜尋**  >  **審核記錄搜尋**] 頁面。</span><span class="sxs-lookup"><span data-stu-id="72cc6-106">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="72cc6-107">在 [**開始日期**] 和 [**結束日期**] 欄位中，選取日期範圍。</span><span class="sxs-lookup"><span data-stu-id="72cc6-107">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="72cc6-108">您不需要指定使用者名稱。</span><span class="sxs-lookup"><span data-stu-id="72cc6-108">You don't need to specify a username.</span></span> <span data-ttu-id="72cc6-109">確認 [**活動**] 欄位已設定為**顯示所有活動的結果**。</span><span class="sxs-lookup"><span data-stu-id="72cc6-109">Verify the **Activities** field is set to **Show results for all activities**.</span></span>

4. <span data-ttu-id="72cc6-110">按一下 [搜尋]。</span><span class="sxs-lookup"><span data-stu-id="72cc6-110">Click **Search**.</span></span>

<span data-ttu-id="72cc6-111">在結果中，按一下 [**篩選結果**]，然後在 [活動篩選] 方塊中輸入**Set-Mailbox** 。</span><span class="sxs-lookup"><span data-stu-id="72cc6-111">In the results, click **Filter Results** and type **Set-Mailbox** in the activity filter box.</span></span> <span data-ttu-id="72cc6-112">選取結果中的審計記錄。</span><span class="sxs-lookup"><span data-stu-id="72cc6-112">Select an audit record in the results.</span></span> <span data-ttu-id="72cc6-113">在 [**詳細資料**] 快顯視窗中，按一下 [**詳細資訊**]。</span><span class="sxs-lookup"><span data-stu-id="72cc6-113">In the **Details** flyout, click **More information**.</span></span> <span data-ttu-id="72cc6-114">您必須查看每個審計記錄的詳細資料，以判斷該活動是否與電子郵件轉寄有關。</span><span class="sxs-lookup"><span data-stu-id="72cc6-114">You have to look at the details of each audit record to determine if the activity is related to email forwarding.</span></span>

- <span data-ttu-id="72cc6-115">**ObjectId**：已修改之信箱的別名值。</span><span class="sxs-lookup"><span data-stu-id="72cc6-115">**ObjectId**: The alias value of the mailbox that was modified.</span></span>

- <span data-ttu-id="72cc6-116">**參數**： _ForwardingSmtpAddress_表示目標電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="72cc6-116">**Parameters**: _ForwardingSmtpAddress_ indicates the target email address.</span></span>

- <span data-ttu-id="72cc6-117">**UserId**：在**ObjectId**欄位中的信箱上設定電子郵件轉寄的使用者。</span><span class="sxs-lookup"><span data-stu-id="72cc6-117">**UserId**: The user who configured email forwarding on the mailbox in the **ObjectId** field.</span></span>

<span data-ttu-id="72cc6-118">如需詳細資訊，請參閱[決定誰設定信箱的電子郵件](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)轉寄功能。</span><span class="sxs-lookup"><span data-stu-id="72cc6-118">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).</span></span>
