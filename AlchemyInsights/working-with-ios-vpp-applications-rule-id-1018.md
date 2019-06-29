---
title: 使用 iOS VPP 應用程式規則識別碼1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 58471f22ce78be1b40d3330a76a92d811819849d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35364835"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 應用程式

請參閱[如何使用 Microsoft intune 的大量購買程式來管理已購買的 iOS 應用程式](https://docs.microsoft.com/intune/vpp-apps-ios), 以瞭解功能、限制, 以及如何使用 Apple 大量購買程式, 以及如何在 Microsoft Intune 中支援。
  
 **常見問題:**「我將 iOS VPP 應用程式指派給我的使用者, 但安裝失敗。」
  
- 如果在多個行動裝置管理提供者上使用單一 VPP 權杖, 就會發生這種情況。 來自 Apple 的 VPP 權杖只能與一個提供者搭配使用。 如果您將 VPP 權杖與多個提供者搭配使用, 則必須將 token 重新上傳至 Intune。

- 如果安裝總數超過授權數目, 安裝也會失敗。 若要查看您的授權使用方式報告, 請移至 [ **Intune 行動應用** \> **程式應用程式授權**] 頁面。 若要瞭解如何收回使用中的授權, 請參閱[本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
