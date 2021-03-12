---
title: 1:1 通話記錄
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733840"
---
# <a name="11-call-recording"></a>1:1 通話記錄

管理員現在必須採取行動，以繼續允許使用者記錄1:1 通話。
 
從2021年4月12日開始，我們將開始強制執行新的小組通話原則選項 *AllowCloudRecordingForCalls*。 

目前1:1 通話記錄功能是由小組會議原則中的 *AllowCloudRecording* 選項所控制。 如果允許使用者記錄小組會議，他們也可以記錄1:1 通話。

如果您想要封鎖所有使用者錄製1:1 通話，您不需要採取任何動作。 *AllowCloudRecordingForCalls* 通話原則選項預設會預設為 $False。

這項變更記錄在下列訊息中心文章中： [ (更新) 1:1 通話記錄原則簡介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) 若要設定小組呼叫原則選項，您必須使用 [團隊 PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)。

**若要在1:1 呼叫中啟用通話記錄：** Set-CsTeamsCallingPolicy 身分識別 Global-AllowCloudRecordingForCalls $True

**停用1:1 通話中的通話記錄：** Set-CsTeamsCallingPolicy 身分識別 Global-AllowCloudRecordingForCalls $False

