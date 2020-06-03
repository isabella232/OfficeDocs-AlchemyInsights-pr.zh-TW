---
title: 啟用封存信箱
ms.author: markjjo
author: markjjo
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "307"
- "3100008"
ms.assetid: e1a5fab7-d3a5-4d4c-8ee2-0edf4ec9b76b
ms.openlocfilehash: 2eecb51a2a6bf2e0741b7ee14dca16f8e0ad4c61
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507017"
---
# <a name="enable-an-archive-mailbox"></a><span data-ttu-id="9e66f-102">啟用封存信箱</span><span class="sxs-lookup"><span data-stu-id="9e66f-102">Enable an archive mailbox</span></span>

<span data-ttu-id="9e66f-103">Microsoft 365 中的封存信箱（也稱為*線上*封存或*In-Place*封存）為使用者提供額外的電子郵件存放區。</span><span class="sxs-lookup"><span data-stu-id="9e66f-103">Archive mailboxes in Microsoft 365 (also called *Online Archives* or *In-Place Archives*) provide users with additional email storage.</span></span> <span data-ttu-id="9e66f-104">使用者可以將專案移動或複製到其封存信箱，系統管理員可以建立可自動將專案移至封存信箱的封存原則。</span><span class="sxs-lookup"><span data-stu-id="9e66f-104">Users can move or copy items to their archive mailbox, and admins can create an archive policy that automatically moves items to archive mailboxes.</span></span>
  
<span data-ttu-id="9e66f-105">以下是建立封存信箱的方式：</span><span class="sxs-lookup"><span data-stu-id="9e66f-105">Here's how to create an archive mailbox:</span></span>
  
1. <span data-ttu-id="9e66f-106">請移至 [https://protection.office.com](https://protection.office.com)。</span><span class="sxs-lookup"><span data-stu-id="9e66f-106">Go to [https://protection.office.com](https://protection.office.com).</span></span>

2. <span data-ttu-id="9e66f-107">使用您的系統管理員帳戶登入 Microsoft 365。</span><span class="sxs-lookup"><span data-stu-id="9e66f-107">Sign in to Microsoft 365 using your admin account.</span></span>

3. <span data-ttu-id="9e66f-108">在安全性與合規性中心的左窗格中 &amp; ，選取 [**資訊管理**封存] \> \*\* \*\*。</span><span class="sxs-lookup"><span data-stu-id="9e66f-108">In the left pane of the Security &amp; Compliance Center, select **Information governance** \> **Archive**.</span></span>

4. <span data-ttu-id="9e66f-109">選取您想要啟用其封存信箱的使用者。</span><span class="sxs-lookup"><span data-stu-id="9e66f-109">Select the user whose archive mailbox you want to enable.</span></span>

5. <span data-ttu-id="9e66f-110">在右側的 [詳細資料] 窗格中，按一下 [**啟用**]，然後在警告訊息中按一下 **[是]** 啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="9e66f-110">In the details pane on the right, click **Enable** and then click **Yes** in the warning message to enable the archive mailbox.</span></span>

<span data-ttu-id="9e66f-111">您也可以選取多個使用者（使用**Shift**或**Ctrl**鍵），然後在詳細資料窗格中按一下 [**啟用**]，以大量啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="9e66f-111">You can also bulk-enable archive mailboxes by selecting multiple users (using the **Shift** or **Ctrl** keys) and then clicking **Enable** in the details pane.</span></span>
  
### <a name="shared-mailboxes"></a><span data-ttu-id="9e66f-112">共用信箱</span><span class="sxs-lookup"><span data-stu-id="9e66f-112">Shared mailboxes</span></span>

<span data-ttu-id="9e66f-113">若要啟用共用信箱的封存，則需要 exchange Online Plan 2 授權或 Exchange online Plan 1 授權與 Exchange Online 封存授權。</span><span class="sxs-lookup"><span data-stu-id="9e66f-113">To enable the archive for a shared mailbox, an Exchange Online Plan 2 license or an Exchange Online Plan 1 license with an Exchange Online Archiving license is required.</span></span>  

<span data-ttu-id="9e66f-114">若要啟用共用信箱的封存：</span><span class="sxs-lookup"><span data-stu-id="9e66f-114">To enable the archive for a shared mailbox:</span></span>

1. <span data-ttu-id="9e66f-115">移至[Exchange 系統管理中心](https://outlook.office365.com/ecp)，並使用您的系統管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="9e66f-115">Go to the [Exchange admin center](https://outlook.office365.com/ecp) and sign in using your admin account.</span></span>

2. <span data-ttu-id="9e66f-116">移至 **[** 共用收件者]  >  \*\* \*\*。</span><span class="sxs-lookup"><span data-stu-id="9e66f-116">Go to **Recipients** > **Shared**.</span></span>

3. <span data-ttu-id="9e66f-117">選取共用信箱。</span><span class="sxs-lookup"><span data-stu-id="9e66f-117">Select the shared mailbox.</span></span>

4. <span data-ttu-id="9e66f-118">在右側的 [詳細資料] 窗格中，按一下 [ **In-Place**封存] 下方的 [**啟用**]，然後按一下 **[是]** 啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="9e66f-118">In the details pane on the right, under **In-Place Archive**, click **Enable**, and then click **Yes** to enable the archive mailbox.</span></span>

<span data-ttu-id="9e66f-119">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="9e66f-119">For more information, see:</span></span>
  
- [<span data-ttu-id="9e66f-120">啟用封存信箱</span><span class="sxs-lookup"><span data-stu-id="9e66f-120">Enable archive mailboxes</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)

- [<span data-ttu-id="9e66f-121">設定封存和刪除原則</span><span class="sxs-lookup"><span data-stu-id="9e66f-121">Set up an archive and deletion policy</span></span>](https://docs.microsoft.com//office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes)
