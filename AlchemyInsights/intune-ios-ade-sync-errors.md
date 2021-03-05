---
title: Apple 自動裝置註冊同步處理錯誤
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448913"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="420ae-102">Apple 自動裝置註冊同步處理錯誤</span><span class="sxs-lookup"><span data-stu-id="420ae-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="420ae-103">"我們已偵測到您有一個或多個已處於錯誤狀態的 ADE/DEP 標記。</span><span class="sxs-lookup"><span data-stu-id="420ae-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="420ae-104">在針對每個受影響的權杖解析錯誤狀態之前，ADE 功能將不會如預期般地運作。</span><span class="sxs-lookup"><span data-stu-id="420ae-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="420ae-105">這項錯誤可能的資訊清單包含下列幾種：</span><span class="sxs-lookup"><span data-stu-id="420ae-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="420ae-106">裝置可能不會從 ABM/ASM 同步至 Intune</span><span class="sxs-lookup"><span data-stu-id="420ae-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="420ae-107">註冊設定檔指派可能失敗</span><span class="sxs-lookup"><span data-stu-id="420ae-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="420ae-108">裝置可能無法順利完成 ADE 註冊</span><span class="sxs-lookup"><span data-stu-id="420ae-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="420ae-109">檢查在 Intune 主控台中的 [裝置 > 註冊裝置] 下是否有報告的同步處理錯誤 **> Apple 註冊 > 註冊計畫標記**。</span><span class="sxs-lookup"><span data-stu-id="420ae-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="420ae-110">同步處理錯誤的其中一個最常見原因是目前的權杖已到期。</span><span class="sxs-lookup"><span data-stu-id="420ae-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="420ae-111">在許多情況下，更新受影響的權杖將會解決問題。</span><span class="sxs-lookup"><span data-stu-id="420ae-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="420ae-112">如果一或多個權杖已到期，請參閱下列檔，以協助您視需要加以更新：</span><span class="sxs-lookup"><span data-stu-id="420ae-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="420ae-113">更新自動裝置註冊權杖</span><span class="sxs-lookup"><span data-stu-id="420ae-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="420ae-114">此外，您還可以查看下列檔，以查看導致權杖同步處理失敗之其他錯誤的可能 remediations：</span><span class="sxs-lookup"><span data-stu-id="420ae-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="420ae-115">IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記</span><span class="sxs-lookup"><span data-stu-id="420ae-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="420ae-116">IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記</span><span class="sxs-lookup"><span data-stu-id="420ae-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
