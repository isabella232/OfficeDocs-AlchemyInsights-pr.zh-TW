---
title: Apple 自動裝置註冊同步處理錯誤
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/17/2020
ms.locfileid: "49707870"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="ec8ed-102">Apple 自動裝置註冊同步處理錯誤</span><span class="sxs-lookup"><span data-stu-id="ec8ed-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="ec8ed-103">"我們已偵測到您有一個或多個已處於錯誤狀態的 ADE/DEP 標記。</span><span class="sxs-lookup"><span data-stu-id="ec8ed-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="ec8ed-104">在針對每個受影響的權杖解析錯誤狀態之前，ADE 功能將不會針對相同的使用。</span><span class="sxs-lookup"><span data-stu-id="ec8ed-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="ec8ed-105">這項錯誤可能的資訊清單包含下列幾種：</span><span class="sxs-lookup"><span data-stu-id="ec8ed-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="ec8ed-106">裝置可能不會從 ABM/ASM 同步至 Intune</span><span class="sxs-lookup"><span data-stu-id="ec8ed-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="ec8ed-107">註冊設定檔指派可能失敗</span><span class="sxs-lookup"><span data-stu-id="ec8ed-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="ec8ed-108">裝置可能無法順利完成 ADE 註冊</span><span class="sxs-lookup"><span data-stu-id="ec8ed-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="ec8ed-109">檢查在 Intune 主控台中的 [裝置 > 登錄 > 裝置] 下的 [裝置註冊裝置] 下的 [同步處理錯誤] **> 註冊計畫權杖** ，並複查下列檔，以查看任何可能的修復：</span><span class="sxs-lookup"><span data-stu-id="ec8ed-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="ec8ed-110">IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記</span><span class="sxs-lookup"><span data-stu-id="ec8ed-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
