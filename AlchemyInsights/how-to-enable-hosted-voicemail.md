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
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055545"
---
# <a name="how-to-enable-hosted-voicemail"></a>如何啟用主控語音信箱

若要啟用語音信箱， **HostedVoicemail** 必須設定為 $true。

使用遠端 PowerShell (RPS) 的使用者上的 **HostedVoicemail** 屬性。

如需連接至 rps 的詳細資訊，請參閱[Microsoft Teams PowerShell 概述](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)，以取得連接至 rps 的詳細資訊。

1. Teams 系統管理員應登入 Teams 的遠端 PowerShell。
1. 從 PowerShell 提示中 Teams Admin 可以執行 **get-csuser user@contoso.com-HostedVoiceMail $true** ，其中的 sip uri 是問題的使用者。

> [!NOTE]
> 對原則所做的變更最多可能需要24小時才能進行複製。