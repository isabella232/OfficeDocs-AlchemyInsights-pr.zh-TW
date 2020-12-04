---
title: 如何在 Outlook for Windows 中新增或移除代理人
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571801"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a><span data-ttu-id="1cc1c-102">如何在 Outlook for Windows 中新增或移除代理人</span><span class="sxs-lookup"><span data-stu-id="1cc1c-102">How to add or remove a Delegate in Outlook for Windows</span></span>

<span data-ttu-id="1cc1c-103">若要在 Outlook for Windows 中新增代理人：</span><span class="sxs-lookup"><span data-stu-id="1cc1c-103">To add a Delegate in Outlook for Windows:</span></span> 

1. <span data-ttu-id="1cc1c-104">依序按一下 [ **檔案] 索引** 標籤及 [ **帳戶設定**]，然後選擇 [ **委派存取**]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-104">Click on the **File** tab followed by **Account Settings**, and then choose **Delegate Access**.</span></span>
2. <span data-ttu-id="1cc1c-105">按一下 [ **新增**]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-105">Click on **Add**.</span></span> <span data-ttu-id="1cc1c-106">如果 [ **新增** ] 不出現，Outlook 和 Exchange 之間可能不會有作用中的連線。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-106">If **Add** doesn’t appear, an active connection might not exist between Outlook and Exchange.</span></span> <span data-ttu-id="1cc1c-107">[Outlook 狀態列] 會顯示上線狀態。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-107">The Outlook status bar displays the connection status.</span></span>
3. <span data-ttu-id="1cc1c-108">輸入您想要指定為代理人的人員名稱，或在搜尋結果清單中選擇名稱。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-108">Type the name of the person you want to designate as your delegate, or search and choose the name in the search results list.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1cc1c-109">代理人必須是組織的 Exchange 全域通訊清單中的人員 (GAL) 。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-109">The delegate must be a person in your organization's Exchange Global Address List (GAL).</span></span>
4. <span data-ttu-id="1cc1c-110">按一下 [ **新增** ]，然後按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-110">Click on **Add** followed by **OK**.</span></span>
5. <span data-ttu-id="1cc1c-111">在 [ **委派許可權** ] 對話方塊中，接受預設許可權設定或選取 [Exchange 資料夾的自訂訪問層級]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-111">In the **Delegate Permissions** dialog box, accept the default permission settings or select custom access levels for Exchange folders.</span></span>

    - <span data-ttu-id="1cc1c-112">若代理人只需要處理會議邀請與回應的許可權，則預設許可權設定（例如代理人）會 **接收傳送給我的會議相關郵件的副本** 。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-112">If a delegate needs permission to work only with meeting requests and responses, the default permission settings such as **Delegate receives copies of meeting-related messages sent to me** are sufficient.</span></span> <span data-ttu-id="1cc1c-113">[ **收件** 匣] 許可權設定可保留 [ **無**]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-113">You can leave the **Inbox** permission setting at **None**.</span></span> <span data-ttu-id="1cc1c-114">會議邀請和回應會直接移至代理人的收件匣。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-114">Meeting requests and responses will go directly to the delegate's inbox.</span></span>

    > [!NOTE]
    > <span data-ttu-id="1cc1c-115">根據預設，授與代理人 **(可以讀取、建立及修改** [行事 **曆** ] 資料夾的專案) 許可權。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-115">By default, the delegate is granted **Editor (can read, create, and modify items)** permission to your **Calendar** folder.</span></span> <span data-ttu-id="1cc1c-116">當代理人代表您回應會議時，它會自動新增至您的 [行事 **曆** ] 資料夾。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-116">When the delegate responds to a meeting on your behalf, it is automatically added to your **Calendar** folder.</span></span>

5. <span data-ttu-id="1cc1c-117">若要傳送郵件以通知代理人已變更的許可權，請選取 [ **自動傳送郵件給代理人摘要這些許可權** ] 核取方塊。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-117">To send a message to notify the delegate of the changed permissions, select the **Automatically send a message to delegate summarizing these permissions** check box.</span></span>
6. <span data-ttu-id="1cc1c-118">如有需要，請選取 [ **代理人可以查看我的私人性質專案** ] 核取方塊。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-118">If you want, select the **Delegate can see my private items** check box.</span></span>

    > [!IMPORTANT]
    > <span data-ttu-id="1cc1c-119">此設定會影響所有 Exchange 資料夾。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-119">This setting affects all Exchange folders.</span></span> <span data-ttu-id="1cc1c-120">這包括所有郵件、連絡人、行事曆、Tasks、記事及日誌資料夾。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-120">This includes all Mail, Contacts, Calendar, Tasks, Notes, and Journal folders.</span></span> <span data-ttu-id="1cc1c-121">沒有任何方法可以只授與指定資料夾中私人專案的存取權。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-121">There is no way to grant access to private items in only specified folders.</span></span>

7. <span data-ttu-id="1cc1c-122">選擇 [確定]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-122">Choose **OK**.</span></span>

    > [!NOTE]
    >
    > - <span data-ttu-id="1cc1c-123">以「代理傳送者」許可權傳送的郵件會在 [ **寄件者**] 旁邊包括代理人和您的名稱。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-123">Messages sent with Send on Behalf permissions include both the delegate's and your names next to **From**.</span></span> <span data-ttu-id="1cc1c-124">當郵件以「以傳送方式傳送」許可權傳送時，只會出現您的名稱。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-124">When a message is sent with Send As permissions, only your name appears.</span></span>
    > - <span data-ttu-id="1cc1c-125">一旦您新增某人做為代理人，他們就可以將您的 Exchange 信箱新增至他們的 Outlook 設定檔。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-125">Once you add someone as a delegate, they can add your Exchange mailbox to their Outlook profile.</span></span> <span data-ttu-id="1cc1c-126">如需相關指示，請參閱 [管理其他人的郵件和行事曆專案](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5)。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-126">For instructions, see [Manage another person's mail and calendar items](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).</span></span>

<span data-ttu-id="1cc1c-127">若要移除 Outlook for Windows 中的代理人：</span><span class="sxs-lookup"><span data-stu-id="1cc1c-127">To remove a Delegate in Outlook for Windows:</span></span>

1. <span data-ttu-id="1cc1c-128">按一下 **[檔案** ] 索引標籤。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-128">Click on the **File** tab.</span></span>
2. <span data-ttu-id="1cc1c-129">按一下 [ **帳戶設定** ]，然後按一下 [ **代理人存取**]。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-129">Click on **Account Settings** followed by **Delegate Access**.</span></span>
3. <span data-ttu-id="1cc1c-130">選擇您要變更許可權的代理人名稱，然後按一下 [ **移除** ] 後再按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="1cc1c-130">Choose the name of the delegate for whom you want to change permissions, and then click on **Remove** followed by **OK**.</span></span>
