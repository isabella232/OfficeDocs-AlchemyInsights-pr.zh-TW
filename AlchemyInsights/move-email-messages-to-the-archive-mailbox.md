---
title: 將電子郵件移至封存信箱
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660366"
---
<span data-ttu-id="7cd81-p101">有問題封存的封存信箱的項目。請確定您已執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="7cd81-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="7cd81-p102">確認的**封存信箱**已啟用。如果不是，使用[本文](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)中的步驟以啟用封存信箱。</span><span class="sxs-lookup"><span data-stu-id="7cd81-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="7cd81-106">在 Exchange 系統管理中心中，選取 [**相符性管理\*\*\*\*保留標記**、 使用 [**移至封存**] 動作包含所需的**保留時間**建立**保留標記**。</span><span class="sxs-lookup"><span data-stu-id="7cd81-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="7cd81-107">在 Exchange 系統管理中心中，選取 [**保留原則**、 建立**保留原則**並新增您**移至封存**保留標記至該原則。</span><span class="sxs-lookup"><span data-stu-id="7cd81-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="7cd81-p103">[將保留原則指派](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)給特定使用者的信箱。將相同的原則會套用至**主要**和**封存**信箱。</span><span class="sxs-lookup"><span data-stu-id="7cd81-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="7cd81-p104">使用者的信箱現在應該有將項目移至封存信箱的封存原則。可能需要強制受管理的資料夾助理員 (MFA) 執行並將新的設定套用至使用者的信箱。執行下列命令以啟動受管理的資料夾助理員特定信箱的同時[連線至 EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) ：</span><span class="sxs-lookup"><span data-stu-id="7cd81-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="7cd81-113">需要設定封存原則的詳細資訊，請參閱[Set up 信箱的封存及刪除原則](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)。</span><span class="sxs-lookup"><span data-stu-id="7cd81-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

