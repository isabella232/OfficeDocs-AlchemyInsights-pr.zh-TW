---
title: 使用 iOS VPP 應用程式規則識別碼1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: f693d12ff0f9c193cba0c6a6802b22d7acd37532c65986e5f6613e18c021f06b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083005"
---
# <a name="working-with-ios-vpp-applications"></a>使用 iOS VPP 應用程式

閱讀[如何使用 Microsoft Intune 來管理透過大量購買程式購買的 iOS app](https://docs.microsoft.com/intune/vpp-apps-ios) ，以瞭解如何使用 Apple volume purchase program，以及如何在 Microsoft Intune 中支援的功能、限制和步驟。
  
 **常見問題：** 「我將 iOS 的 VPP 應用程式指派給我的使用者，但是安裝失敗。」
  
- 如果您跨多個行動裝置管理提供者使用單一 VPP 權杖，便會發生這種情況。 來自 Apple 的 VPP 權杖只會與一個提供者搭配使用。 如果您使用的 VPP 權杖與多個提供者，則必須將權杖重新上傳至 Intune。

- 如果安裝總數超過授權數目，也可能會失敗。 若要查看授權的流量報告，請移至 [ **Intune 行動應用** 程式 \> **應用程式授權** ] 頁面。 若要瞭解如何回收使用中的授權，請參閱 [本文。](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
