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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 自動裝置註冊同步處理錯誤

"我們已偵測到您有一個或多個已處於錯誤狀態的 ADE/DEP 標記。 在針對每個受影響的權杖解析錯誤狀態之前，ADE 功能將不會如預期般地運作。

這項錯誤可能的資訊清單包含下列幾種：

1. 裝置可能不會從 ABM/ASM 同步至 Intune
2. 註冊設定檔指派可能失敗
3. 裝置可能無法順利完成 ADE 註冊

檢查在 Intune 主控台中的 [裝置 > 註冊裝置] 下是否有報告的同步處理錯誤 **> Apple 註冊 > 註冊計畫標記**。

同步處理錯誤的其中一個最常見原因是目前的權杖已到期。 在許多情況下，更新受影響的權杖將會解決問題。

如果一或多個權杖已到期，請參閱下列檔，以協助您視需要加以更新：

[更新自動裝置註冊權杖](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

此外，您還可以查看下列檔，以查看導致權杖同步處理失敗之其他錯誤的可能 remediations：

[IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
