---
title: 監視的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 374814f4eabd61433a15876ebf7f351819933c21
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36538732"
---
# <a name="monitoring-conditional-access-for-exchange"></a>監視 Exchange 的條件式存取

使用條件式存取目標使用者會收到通知電子郵件，如果未符合您的組織存取需求。 若要解決，我們建議一或多個下列解決方案：
  
- 如果裝置會假設要註冊，通知使用者前往的公司入口網站應用程式，並確認它會出現在公司入口網站。 如果沒有，則使用者應該註冊裝置。
    
- 在 Azure 入口網站移至**Intune\>裝置相容性**。 在 [**監視**] 下按一下 [**裝置相容性**]。 檢視裝置合規性報告，以確認使用者的裝置標記為相容。 
    
- 在 Azure 入口網站移至**Intune\>裝置相容性**。 在 [**管理**] 下按一下 [**原則**]。 在符合性原則清單中，確認設定檔指派給使用者的裝置。 如果沒有設定檔指派，然後 Intune 將無法確認裝置的合規性狀態。 
    
- 編輯使用者的條件式存取工作分派。
    
1. 在 Azure 入口網站移至 [ **Intune\>條件式存取\>原則**
    
2. 從清單中選取原則
    
3. 按一下 [**使用者和群組**
    
4. 若要為目標的特定原則的人員，請將其新增至 [**包含**清單中。 若要確保人員省略從原則，請將其新增至**排除**清單中。 
    
閱讀其他資訊：[如何監視條件式存取裝置](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

