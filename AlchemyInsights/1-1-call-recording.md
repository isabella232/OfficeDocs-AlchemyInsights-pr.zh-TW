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
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696913"
---
# <a name="11-call-recording"></a><span data-ttu-id="cfa66-102">1:1 通話記錄</span><span class="sxs-lookup"><span data-stu-id="cfa66-102">1:1 call recording</span></span>

<span data-ttu-id="cfa66-103">如果 [ **開始錄製** ] 按鈕在1:1 呼叫中呈現為灰色，您必須變更受影響使用者的原則設定。</span><span class="sxs-lookup"><span data-stu-id="cfa66-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="cfa66-104">2021年5月31日，我們將開始強制執行新的 Teams 呼叫原則 *AllowCloudRecordingForCalls*。</span><span class="sxs-lookup"><span data-stu-id="cfa66-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="cfa66-105">在此變更之前，1:1 通話記錄是由 *AllowCloudRecording* Teams 會議原則所控制。</span><span class="sxs-lookup"><span data-stu-id="cfa66-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="cfa66-106">這項變更會記錄在訊息中心文章中： [ (已更新) 1:1 通話記錄原則簡介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)。</span><span class="sxs-lookup"><span data-stu-id="cfa66-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="cfa66-107">*AllowCloudRecordingForCalls*  通話原則選項預設設為 **$False** 。</span><span class="sxs-lookup"><span data-stu-id="cfa66-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="cfa66-108">如果您想要封鎖所有使用者錄製1:1 通話，您不需要採取任何動作。</span><span class="sxs-lookup"><span data-stu-id="cfa66-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="cfa66-109">若要為1:1 呼叫中的所有使用者啟用通話記錄，請使用 Teams PowerShell 執行下列 Cmdlet：</span><span class="sxs-lookup"><span data-stu-id="cfa66-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="cfa66-110">**Set-CsTeamsCallingPolicy-Identity Global-AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="cfa66-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="cfa66-111">或者，您也可以建立新的原則並設定 **AllowCloudRecordingForCalls** **$true** ，並將該原則指派給您的使用者。</span><span class="sxs-lookup"><span data-stu-id="cfa66-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="cfa66-112">如需詳細資訊，請 [1:1 參閱這裡 () 的通話記錄原則控制！這裡](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668)。</span><span class="sxs-lookup"><span data-stu-id="cfa66-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
