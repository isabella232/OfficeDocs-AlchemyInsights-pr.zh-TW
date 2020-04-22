---
title: 監視條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 8b76d58791408037b5704b421d7afa166e3ea0be
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713709"
---
# <a name="monitoring-conditional-access-for-exchange"></a>監視 Exchange 的條件式存取

以條件式存取為目標的使用者，如果不符合您組織的存取需求，將會收到通知電子郵件。 若要解決此問題，我們建議下列一或多個解決方案：
  
- 若要對裝置進行註冊，請建議使用者移至公司入口網站，並確認該應用程式出現在公司入口網站。 如果不是，則使用者應該註冊裝置。
    
- 在 Azure 入口網站中，移至** \> Intune 裝置規範**。 在 [**監視器**] 底下按一下 [**裝置符合性**]。 查看您的裝置符合性報告，以確認使用者的裝置已標示為相容。 
    
- 在 Azure 入口網站中，移至** \> Intune 裝置規範**。 在 [**管理**] 下，按一下 [**原則**]。 在 [規範原則] 清單中，確認已將設定檔指派給您的使用者裝置。 若未指派設定檔，則 Intune 將無法確認裝置的符合性狀態。 
    
- 編輯使用者的條件式存取指派。
    
1. 在 Azure 入口網站移至**Intune \>條件式\>存取原則**
    
2. 從清單中選取原則
    
3. 按一下 [**使用者和群組**]
    
4. 若要以某人為目標設定特定原則，請將其新增至 [**包含**] 清單。 若要確保從原則中省略了某個人員，請將其新增至 [**排除**] 清單。 
    
閱讀其他資訊：[如何監視條件式存取裝置](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

