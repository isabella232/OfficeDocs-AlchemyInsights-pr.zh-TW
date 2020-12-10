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
# <a name="how-to-enable-hosted-voicemail"></a>如何啟用主控語音信箱

若要啟用語音信箱， **HostedVoicemail** 必須設定為 $true。

使用遠端 PowerShell (RPS) 的使用者上的 **HostedVoicemail** 屬性。

如需連接至 RPS 的詳細資訊，請參閱 [Microsoft 團隊 PowerShell 一覽](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) ，以取得連線至 rps 的詳細資訊。

1. 小組管理員應該登入小組的遠端 PowerShell。
1. 從 PowerShell 提示小組管理員可以執行 **get-csuser user@contoso.com-HostedVoiceMail $true** （sip uri 屬於問題使用者）。

> [!NOTE]
> 對原則所做的變更最多可能需要24小時才能進行複製。