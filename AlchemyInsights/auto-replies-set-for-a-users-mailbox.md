---
title: 設定信箱的自動回覆
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 60af581e7fe508ab9644a53873bcd551b3aacff1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820925"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="3a2a9-102">為使用者信箱設定自動回覆</span><span class="sxs-lookup"><span data-stu-id="3a2a9-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="3a2a9-103">**方法 1**</span><span class="sxs-lookup"><span data-stu-id="3a2a9-103">**Method 1**</span></span>

1. <span data-ttu-id="3a2a9-104">登入 Microsoft 365 入口網站。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="3a2a9-105">移至 [使用者] > [作用中使用者] (如果您在共用信箱上進行設定，則移至或 [群組] > [共用信箱])。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="3a2a9-106">選取擁有 Microsoft Exchange 信箱的使用者。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="3a2a9-107">在右側的飛出功能表中，移至 [郵件設定] > [自動回覆] (如果這是共用信箱，只要按一下飛出功能表上的 [自動回覆] 即可)。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="3a2a9-108">**方法 2**</span><span class="sxs-lookup"><span data-stu-id="3a2a9-108">**Method 2**</span></span>

1. <span data-ttu-id="3a2a9-109">使用系統管理員認證登入 Microsoft 365 系統管理入口網站。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="3a2a9-110">展開 [系統管理中心]，然後按一下 [Exchange]。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="3a2a9-111">按一下右上角的圖片、按一下 [其他使用者]，然後選取您要變更的使用者信箱。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="3a2a9-112">在左側選取 [選項]、按一下 [組織電子郵件]，再按一下 [自動回覆]。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="3a2a9-113">**方法 3**</span><span class="sxs-lookup"><span data-stu-id="3a2a9-113">**Method 3**</span></span>

<span data-ttu-id="3a2a9-114">在 Exchange Online PowerShell 中執行下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="3a2a9-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="3a2a9-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="3a2a9-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="3a2a9-116">如需有關此 Cmdlet 的詳細資訊，請參閱 [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration) (英文)。</span><span class="sxs-lookup"><span data-stu-id="3a2a9-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
