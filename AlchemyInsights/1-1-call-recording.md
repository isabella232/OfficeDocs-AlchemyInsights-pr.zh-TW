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
# <a name="11-call-recording"></a><span data-ttu-id="4cf94-102">1:1 通話記錄</span><span class="sxs-lookup"><span data-stu-id="4cf94-102">1:1 call recording</span></span>

<span data-ttu-id="4cf94-103">管理員現在必須採取行動，以繼續允許使用者記錄1:1 通話。</span><span class="sxs-lookup"><span data-stu-id="4cf94-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="4cf94-104">從2021年4月12日開始，我們將開始強制執行新的小組通話原則選項 *AllowCloudRecordingForCalls*。</span><span class="sxs-lookup"><span data-stu-id="4cf94-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="4cf94-105">目前1:1 通話記錄功能是由小組會議原則中的 *AllowCloudRecording* 選項所控制。</span><span class="sxs-lookup"><span data-stu-id="4cf94-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="4cf94-106">如果允許使用者記錄小組會議，他們也可以記錄1:1 通話。</span><span class="sxs-lookup"><span data-stu-id="4cf94-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="4cf94-107">如果您想要封鎖所有使用者錄製1:1 通話，您不需要採取任何動作。</span><span class="sxs-lookup"><span data-stu-id="4cf94-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="4cf94-108">*AllowCloudRecordingForCalls* 通話原則選項預設會預設為 $False。</span><span class="sxs-lookup"><span data-stu-id="4cf94-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="4cf94-109">這項變更記錄在下列訊息中心文章中： [ (更新) 1:1 通話記錄原則簡介](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) 若要設定小組呼叫原則選項，您必須使用 [團隊 PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install)。</span><span class="sxs-lookup"><span data-stu-id="4cf94-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="4cf94-110">**若要在1:1 呼叫中啟用通話記錄：** Set-CsTeamsCallingPolicy 身分識別 Global-AllowCloudRecordingForCalls $True</span><span class="sxs-lookup"><span data-stu-id="4cf94-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="4cf94-111">**停用1:1 通話中的通話記錄：** Set-CsTeamsCallingPolicy 身分識別 Global-AllowCloudRecordingForCalls $False</span><span class="sxs-lookup"><span data-stu-id="4cf94-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

