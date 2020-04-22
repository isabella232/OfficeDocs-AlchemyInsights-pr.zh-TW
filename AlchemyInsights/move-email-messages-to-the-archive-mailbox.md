---
title: 將電子郵件訊息移至封存信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a5ad81e97df0ed5c337a622126173df94af80bb8
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713637"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="d9220-102">將電子郵件移至封存信箱</span><span class="sxs-lookup"><span data-stu-id="d9220-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="d9220-103">確認已啟用封存**信箱**。</span><span class="sxs-lookup"><span data-stu-id="d9220-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="d9220-104">如果不是，請使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步驟來啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="d9220-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="d9220-105">若要將郵件自動封存到封存信箱，必須將具有 [**移至**封存] 動作的保留標記設定為 [**自動套用至整個信箱（預設）] 標記**。</span><span class="sxs-lookup"><span data-stu-id="d9220-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="d9220-106">使用這裡的步驟來建立標記：封存[預設](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)標籤。</span><span class="sxs-lookup"><span data-stu-id="d9220-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="d9220-107">接下來，將**Archive**封存標籤新增至保留原則。</span><span class="sxs-lookup"><span data-stu-id="d9220-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="d9220-108">在 Exchange 系統管理中心中，選擇 [**保留原則**] > 將 [**移至**封存] 標記新增至原則 >**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="d9220-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="d9220-109">現在[將保留原則指派](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="d9220-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="d9220-110">相同的原則會同時套用至**主要**和**封存信箱。**</span><span class="sxs-lookup"><span data-stu-id="d9220-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="d9220-111">您可能需要強制受管理的資料夾助理（MFA）執行，並將新的設定套用至使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="d9220-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="d9220-112">在[連線至 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)時執行下列命令，以啟動特定信箱的受管理的資料夾助理：</span><span class="sxs-lookup"><span data-stu-id="d9220-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="d9220-113">Start-ManagedFolderAssistant 身分識別<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="d9220-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="d9220-114">如需設定封存原則的詳細資訊，請參閱[設定信箱的封存和刪除原則](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。</span><span class="sxs-lookup"><span data-stu-id="d9220-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  