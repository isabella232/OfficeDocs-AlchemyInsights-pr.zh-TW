---
title: 使用 iOS VPP 應用程式規則 Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420475"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 應用程式

閱讀[如何管理 iOS 應用程式以透過使用 Microsoft Intune 大量購買方案購買](https://docs.microsoft.com/intune/vpp-apps-ios)若要了解功能、 限制和步驟，才能建立使用 Apple 大量購買方案和為其 Microsoft Intune 中的支援。 
  
 **常見的問題：**「 我 iOS VPP app 給我的使用者，但安裝失敗 」。 
  
- 如果是單一 VPP 語彙基元跨越多個行動裝置管理提供者，這可能會發生。 來自 Apple 的 VPP 權杖僅搭配一個提供者。 如果您使用多個提供者使用 VPP 語彙基元，您必須重新上傳到 Intune 的語彙基元。
    
- 如果安裝總數量超過授權數量，也會失敗的安裝。 若要檢視您的授權的流量報告，請前往 [ **Intune 行動應用程式** \> **應用程式授權**] 頁面。 若要了解如何收回中使用的授權，請參閱[這篇文章。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
    

