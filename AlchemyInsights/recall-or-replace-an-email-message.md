---
title: 召回或取代電子郵件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353497"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="02b68-102">召回或取代 Microsoft 365 中的電子郵件</span><span class="sxs-lookup"><span data-stu-id="02b68-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="02b68-103">您 **只能召回傳送給組織中人員的郵件**。</span><span class="sxs-lookup"><span data-stu-id="02b68-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="02b68-104">例如，如果郵件已傳送至 Gmail 位址，您就無法將它重新叫用。</span><span class="sxs-lookup"><span data-stu-id="02b68-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="02b68-105">您 **只能召回從 Outlook 傳送給電腦的郵件**。</span><span class="sxs-lookup"><span data-stu-id="02b68-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="02b68-106">如果使用者使用 Outlook for Mac 或 web 上的 Outlook 傳送郵件，您就無法將其重新叫用。</span><span class="sxs-lookup"><span data-stu-id="02b68-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="02b68-107">作為租使用者系統管理員，您可以 **使用 PowerShell (來代表使用者重新叫用郵件** 。如需詳細資訊，請參閱： [搜尋並刪除電子郵件訊息](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)) 。</span><span class="sxs-lookup"><span data-stu-id="02b68-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="02b68-108">您無法從系統管理中心重新叫用郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="02b68-109">向內滾動至「搜尋並刪除組織中的電子郵件」，以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="02b68-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="02b68-110">**召回或取代您傳送的電子郵件**</span><span class="sxs-lookup"><span data-stu-id="02b68-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="02b68-111">在 Outlook 視窗左側的 [資料夾] 窗格中，選擇 [送出的專案] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="02b68-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="02b68-112">開啟您要撤回的郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-112">Open the message that you want to recall.</span></span> <span data-ttu-id="02b68-113">您必須按兩下以開啟郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-113">You must double-click to open the message.</span></span> <span data-ttu-id="02b68-114">選取郵件，使其出現在讀取窗格中，就不會讓您想起郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="02b68-115">從 [郵件] 索引標籤中，選取 [**動作**  >  **撤回此郵件**]。</span><span class="sxs-lookup"><span data-stu-id="02b68-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="02b68-116">選擇 [ **刪除此郵件的未讀副本** ] 或 [ **刪除未讀取的副本並以新郵件取代**]，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="02b68-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="02b68-117">如果您要傳送取代郵件，請撰寫郵件，然後選取 [ **傳送**]。</span><span class="sxs-lookup"><span data-stu-id="02b68-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="02b68-118">郵件召回的成功或失敗取決於 Outlook 中的收件者設定。</span><span class="sxs-lookup"><span data-stu-id="02b68-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="02b68-119">如需詳細資訊，包括如何檢查召回，請參閱 [召回或取代您傳送的電子](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="02b68-120">**_若要在您的組織中搜尋並刪除電子郵件訊息_**，當您是全域系統管理員時，它會是最簡單的方法。如果您不是全域系統管理員，則必須將您的帳戶新增至 eDiscovery 管理員角色群組，或「符合性搜尋管理」角色。</span><span class="sxs-lookup"><span data-stu-id="02b68-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="02b68-121">若要刪除郵件，您需要加入「組織管理」角色群組或「搜尋並清除」管理角色。</span><span class="sxs-lookup"><span data-stu-id="02b68-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="02b68-122">在 [安全性 & 規範中心](https://protection.office.com/)指派這些角色的許可權。</span><span class="sxs-lookup"><span data-stu-id="02b68-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="02b68-123">[建立內容搜尋](https://docs.microsoft.com/microsoft-365/compliance/content-search) ，以尋找要刪除的郵件。</span><span class="sxs-lookup"><span data-stu-id="02b68-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="02b68-124">[連線到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="02b68-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="02b68-125">如果您使用 MFA (多重要素驗證) ，請參閱 [使用多重要素驗證連線至 Microsoft 365 Security & 規範中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="02b68-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
