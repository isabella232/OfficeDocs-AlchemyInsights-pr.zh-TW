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
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple 自動裝置註冊同步處理錯誤

"我們已偵測到您有一個或多個已處於錯誤狀態的 ADE/DEP 標記。 在針對每個受影響的權杖解析錯誤狀態之前，ADE 功能將不會針對相同的使用。

這項錯誤可能的資訊清單包含下列幾種：

1. 裝置可能不會從 ABM/ASM 同步至 Intune
2. 註冊設定檔指派可能失敗
3. 裝置可能無法順利完成 ADE 註冊

檢查在 Intune 主控台中的 [裝置 > 登錄 > 裝置] 下的 [裝置註冊裝置] 下的 [同步處理錯誤] **> 註冊計畫權杖** ，並複查下列檔，以查看任何可能的修復：

[IOS/iPadOS 的 ABM/ASM 同步處理錯誤，以及 macOS 自動裝置註冊標記](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
