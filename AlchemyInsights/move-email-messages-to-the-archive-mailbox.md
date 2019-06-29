---
title: 將電子郵件移至封存信箱
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: a29fb799b68f5c187ca1d44aeaf94e6cd8760b0e
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35379488"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="ffc64-102">將電子郵件移至封存信箱</span><span class="sxs-lookup"><span data-stu-id="ffc64-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="ffc64-103">確認已啟用封存**信箱**。</span><span class="sxs-lookup"><span data-stu-id="ffc64-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="ffc64-104">如果不是, 請使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步驟來啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="ffc64-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="ffc64-105">若要將郵件自動封存至封存信箱, 必須將保留標記設為 [**移至**封存] 動作, 才能**自動套用至整個信箱 (預設) 標記**。</span><span class="sxs-lookup"><span data-stu-id="ffc64-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="ffc64-106">使用此處的步驟來建立標記: [Archive Default 標記](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)。</span><span class="sxs-lookup"><span data-stu-id="ffc64-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>

3. <span data-ttu-id="ffc64-107">接下來, 將\*\*\*\* 封存標籤新增至您的保留原則。</span><span class="sxs-lookup"><span data-stu-id="ffc64-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="ffc64-108">在 Exchange 系統管理中心, 選擇 [**保留原則**] > 將 [**移至**封存] 標記新增至 [原則] >**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="ffc64-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="ffc64-109">現在,[將保留原則指派](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="ffc64-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="ffc64-110">相同的原則會同時套用至**主要**和封存信箱。 \*\*\*\*</span><span class="sxs-lookup"><span data-stu-id="ffc64-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="ffc64-111">您可能需要強制受管理的資料夾助理 (MFA) 執行, 並將新的設定套用至使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="ffc64-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="ffc64-112">[連線至 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)以啟動特定信箱的受管理的資料夾助理時, 請執行下列命令:</span><span class="sxs-lookup"><span data-stu-id="ffc64-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="ffc64-113">啟動-ManagedFolderAssistant-Identity<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="ffc64-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="ffc64-114">如需設定封存原則的詳細資訊, 請參閱[設定信箱的封存和刪除原則](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。</span><span class="sxs-lookup"><span data-stu-id="ffc64-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  