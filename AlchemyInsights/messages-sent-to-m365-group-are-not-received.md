---
title: 所有成員都不會收到傳送到 Microsoft 365 群組的郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: d222eb92d806bad52264139a8ddba72f323b3783
ms.sourcegitcommit: 10cfd9d552b0d8a096bcef34e82c04a4c166a13a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/05/2021
ms.locfileid: "50479444"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="06eba-102">所有成員都不會收到傳送到 Microsoft 365 群組的郵件</span><span class="sxs-lookup"><span data-stu-id="06eba-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="06eba-103">請確定所有群組成員都已訂閱，以接收電子郵件。</span><span class="sxs-lookup"><span data-stu-id="06eba-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="06eba-104">請參閱[追蹤 Outlook 中的群組](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)。</span><span class="sxs-lookup"><span data-stu-id="06eba-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="06eba-105">若要檢查已訂閱群組電子郵件的成員的郵件狀態，請在 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true) 上執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="06eba-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="06eba-106">使用下列 EXO PowerShell 命令以設定所有群組成員在其收件夾中接收傳送至 Microsoft 365 群組的電子郵件：</span><span class="sxs-lookup"><span data-stu-id="06eba-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

<span data-ttu-id="06eba-107">例如：</span><span class="sxs-lookup"><span data-stu-id="06eba-107">For example:</span></span>

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`