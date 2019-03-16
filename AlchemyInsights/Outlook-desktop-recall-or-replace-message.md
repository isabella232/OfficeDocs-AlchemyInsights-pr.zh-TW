---
title: Outlook 桌面回收] 或 [取代電子郵件訊息
ms.author: daeite
author: daeite
manager: joallard
ms.date: 3/13/2019
ms.audience: Admin
ms.topic: article
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: aced684777ef82860b969aea8825699b78b04c5a
ms.sourcegitcommit: aad9f863bc9fd7d5522c480bd1a7d15f3a80ff4f
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/15/2019
ms.locfileid: "30657035"
---
# <a name="recall-or-replace-an-email-message"></a><span data-ttu-id="c2e44-102">回收或取代的電子郵件訊息</span><span class="sxs-lookup"><span data-stu-id="c2e44-102">Recall or replace an email message</span></span>

- <span data-ttu-id="c2e44-103">身為系統管理員，您還可以**代表使用者使用 PowerShell 重新叫用郵件**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="c2e44-104">您無法回收從管理中心的郵件。</span><span class="sxs-lookup"><span data-stu-id="c2e44-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="c2e44-105">您可以**只重新叫用郵件，傳送給您組織中的人員**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="c2e44-106">如果郵件已傳送到 Gmail 地址，例如，您無法恢復它。</span><span class="sxs-lookup"><span data-stu-id="c2e44-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="c2e44-107">您可以**只會重新叫用從 Outlook 2016 在 PC 上傳送的郵件**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="c2e44-108">如果使用者傳送郵件，使用 Mac 版 Outlook 或網頁型 Outlook，您就無法再回收。</span><span class="sxs-lookup"><span data-stu-id="c2e44-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="c2e44-109">若要恢復或取代的電子郵件訊息：</span><span class="sxs-lookup"><span data-stu-id="c2e44-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="c2e44-110">在 [Outlook 視窗左側的 [資料夾] 窗格中，選取 [寄件備份] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="c2e44-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="c2e44-111">連按兩下您想要回收以開啟的郵件。</span><span class="sxs-lookup"><span data-stu-id="c2e44-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="c2e44-112">選取 [**郵件**] 索引標籤，然後選取 [**動作** > **回收這封郵件**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="c2e44-113">選取 [**刪除此郵件未讀取**或**刪除未閱讀的郵件，並取代為新的郵件**]，然後選取 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="c2e44-114">如果您正在傳送替換訊息，撰寫郵件，，，，然後選取 [**傳送**。</span><span class="sxs-lookup"><span data-stu-id="c2e44-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="c2e44-115">成功或失敗的訊息重新叫用取決於 Outlook 中的收件者的設定。</span><span class="sxs-lookup"><span data-stu-id="c2e44-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="c2e44-116">若要查看重新叫用的步驟，請參閱[這篇文章](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)。</span><span class="sxs-lookup"><span data-stu-id="c2e44-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="c2e44-117">搜尋並刪除您的組織中的電子郵件</span><span class="sxs-lookup"><span data-stu-id="c2e44-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="c2e44-118">如果您不是全域系統管理員，您的帳戶必須新增至 eDiscovery 管理員 」 角色或符合性搜尋來搜尋郵件的管理角色。</span><span class="sxs-lookup"><span data-stu-id="c2e44-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="c2e44-119">若要刪除的郵件，您需要加入 「 組織管理 」 角色群組或 「 搜尋及清除的 「 管理 」 角色。</span><span class="sxs-lookup"><span data-stu-id="c2e44-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="c2e44-120">在[安全性與合規性中心](https://go.microsoft.com/fwlink/?linkid=2083731)指派這些角色的權限。</span><span class="sxs-lookup"><span data-stu-id="c2e44-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="c2e44-121">[建立內容搜尋](https://docs.microsoft.com/office365/securitycompliance/content-search)來尋找要刪除的郵件。</span><span class="sxs-lookup"><span data-stu-id="c2e44-121">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="c2e44-122">[連接到安全性與合規性中心 PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps)。</span><span class="sxs-lookup"><span data-stu-id="c2e44-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="c2e44-123">如果您使用多重要素驗證，請參閱 < <b0>Connect to Office 365 安全性與合規性中心 PowerShell 中使用多重要素驗證</b0>。</span><span class="sxs-lookup"><span data-stu-id="c2e44-123">If you're using multi-factor authentication, see [Connect to Office 365 Security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>