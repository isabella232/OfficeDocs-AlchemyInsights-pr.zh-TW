---
title: 如何啟用主控語音信箱
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/09/2020
ms.locfileid: "49608828"
---
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="8b910-102">如何啟用主控語音信箱</span><span class="sxs-lookup"><span data-stu-id="8b910-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="8b910-103">若要啟用語音信箱， **HostedVoicemail** 必須設定為 $true。</span><span class="sxs-lookup"><span data-stu-id="8b910-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="8b910-104">使用遠端 PowerShell (RPS) 的使用者上的 **HostedVoicemail** 屬性。</span><span class="sxs-lookup"><span data-stu-id="8b910-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="8b910-105">如需連接至 RPS 的詳細資訊，請參閱 [Microsoft 團隊 PowerShell 一覽](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) ，以取得連線至 rps 的詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="8b910-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="8b910-106">小組管理員應該登入小組的遠端 PowerShell。</span><span class="sxs-lookup"><span data-stu-id="8b910-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="8b910-107">從 PowerShell 提示小組管理員可以執行 **get-csuser user@contoso.com-HostedVoiceMail $true** （sip uri 屬於問題使用者）。</span><span class="sxs-lookup"><span data-stu-id="8b910-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="8b910-108">對原則所做的變更最多可能需要24小時才能進行複製。</span><span class="sxs-lookup"><span data-stu-id="8b910-108">Changes to policies can take up to 24 hours to replicate.</span></span>