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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702081"
---
# <a name="11-call-recording"></a>1:1 通話記錄

如果 [ **開始錄製** ] 按鈕在1:1 呼叫中呈現為灰色，您必須變更受影響使用者的原則設定。 若要檢查原則設定，請輸入下列命令，以執行受影響使用者的診斷：請輸入上方的 [**診斷： Teams 1:1 通話記錄**]。     

2021年5月31日，我們將開始強制執行新的 Teams 呼叫原則 *AllowCloudRecordingForCalls*。 在此變更之前，1:1 通話記錄是由 *AllowCloudRecording* Teams 會議原則所控制。 這項變更會記錄在訊息中心文章中： [ (已更新) 1:1 通話記錄原則簡介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。  

*AllowCloudRecordingForCalls*  通話原則選項預設設為 **$False** 。 如果您想要封鎖所有使用者錄製1:1 通話，您不需要採取任何動作。  

若要為1:1 呼叫中的所有使用者啟用通話記錄，請使用 [Teams PowerShell](/microsoftteams/teams-powershell-install)執行下列 Cmdlet： 

**Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True** 

或者，您也可以建立新的原則並設定 **AllowCloudRecordingForCalls** **$true** ，並將該原則指派給您的使用者。 

如需詳細資訊，請 [1:1 參閱這裡 () 的通話記錄原則控制！這裡](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)。
