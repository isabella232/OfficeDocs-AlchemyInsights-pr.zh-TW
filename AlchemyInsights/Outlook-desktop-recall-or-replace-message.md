---
title: Outlook 桌面召回或取代電子郵件
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: d64332778f9132aff6a9660bb0d522f4e16b753c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687501"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="16bbc-102">召回或取代 Outlook 電子郵件</span><span class="sxs-lookup"><span data-stu-id="16bbc-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="16bbc-103">作為管理員，您可以**代表使用者使用 PowerShell 撤回郵件**。</span><span class="sxs-lookup"><span data-stu-id="16bbc-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="16bbc-104">您無法從系統管理中心重新叫用郵件。</span><span class="sxs-lookup"><span data-stu-id="16bbc-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="16bbc-105">您**只能召回傳送給組織中人員的郵件**。</span><span class="sxs-lookup"><span data-stu-id="16bbc-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="16bbc-106">例如，如果郵件已傳送至 Gmail 位址，您就無法將其重新叫用。</span><span class="sxs-lookup"><span data-stu-id="16bbc-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="16bbc-107">您**只能撤銷從電腦上的 Outlook 2016 傳送的郵件**。</span><span class="sxs-lookup"><span data-stu-id="16bbc-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="16bbc-108">如果使用者使用 Outlook for Mac 或 web 上的 Outlook 傳送郵件，您就無法將其重新叫用。</span><span class="sxs-lookup"><span data-stu-id="16bbc-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="16bbc-109">若要撤回或取代電子郵件：</span><span class="sxs-lookup"><span data-stu-id="16bbc-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="16bbc-110">在 Outlook 視窗左側的 [資料夾] 窗格中，選取 [寄件備份] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="16bbc-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="16bbc-111">按兩下您要重新開啟的郵件。</span><span class="sxs-lookup"><span data-stu-id="16bbc-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="16bbc-112">選取 [**郵件**] 索引標籤，然後選取 [**動作** > ] [重新**叫用此郵件**]。</span><span class="sxs-lookup"><span data-stu-id="16bbc-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="16bbc-113">選取 [**刪除此郵件的未讀副本**] 或 [**刪除未讀取的副本並以新郵件取代**]，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="16bbc-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="16bbc-114">如果您正在傳送取代郵件，請撰寫郵件，然後選取 [**傳送**]。</span><span class="sxs-lookup"><span data-stu-id="16bbc-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="16bbc-115">郵件召回的成功或失敗取決於 Outlook 中收件者的設定。</span><span class="sxs-lookup"><span data-stu-id="16bbc-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="16bbc-116">如需檢查重新叫用的步驟，請參閱[本文](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。</span><span class="sxs-lookup"><span data-stu-id="16bbc-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="16bbc-117">搜尋並刪除組織中的電子郵件</span><span class="sxs-lookup"><span data-stu-id="16bbc-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="16bbc-118">如果您不是全域系統管理員，則必須將您的帳戶新增至「eDiscovery 管理員」角色或「符合性搜尋管理」角色，才能搜尋郵件。</span><span class="sxs-lookup"><span data-stu-id="16bbc-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="16bbc-119">若要刪除郵件，您需要加入「組織管理」角色群組或「搜尋並清除」管理角色。</span><span class="sxs-lookup"><span data-stu-id="16bbc-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="16bbc-120">在 [[安全性與合規性中心](https://go.microsoft.com/fwlink/?linkid=2083731)] 中指派這些角色的許可權。</span><span class="sxs-lookup"><span data-stu-id="16bbc-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="16bbc-121">[建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search)，以尋找要刪除的郵件。</span><span class="sxs-lookup"><span data-stu-id="16bbc-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="16bbc-122">[連接到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="16bbc-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="16bbc-123">如果您使用的是多重要素驗證，請參閱[使用多重要素驗證連線至 Microsoft 365 安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="16bbc-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>