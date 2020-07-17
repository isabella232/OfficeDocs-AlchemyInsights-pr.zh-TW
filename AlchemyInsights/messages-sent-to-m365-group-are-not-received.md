---
title: 所有成員都不會收到傳送到 Microsoft 365 群組的郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/06/2020
ms.locfileid: "45047230"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="708e3-102">所有成員都不會收到傳送到 Microsoft 365 群組的郵件</span><span class="sxs-lookup"><span data-stu-id="708e3-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="708e3-103">請確定所有群組成員都已訂閱，以接收電子郵件。</span><span class="sxs-lookup"><span data-stu-id="708e3-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="708e3-104">請參閱[追蹤 Outlook 中的群組](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36)。</span><span class="sxs-lookup"><span data-stu-id="708e3-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="708e3-105">若要檢查已訂閱群組電子郵件的成員的郵件狀態，請在 [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps) 上執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="708e3-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`