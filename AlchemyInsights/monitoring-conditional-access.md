---
title: 監視設定格式化的條件的存取
ms.author: pebaum
author: pebaum
ms.date: 8/1/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 756c5e98ed3e9cedd0152b5747ea6bf1ed31778e
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29902332"
---
# <a name="monitoring-conditional-access"></a>監視設定格式化的條件的存取

針對設定格式化的條件的存取權的使用者會收到通知電子郵件不符合您的組織存取需求。若要解決，我們建議一或多個下列解決方案：
  
- 如果裝置假設是以註冊，通知使用者移至的公司入口網站應用程式，並確認其出現在公司入口網站。如果它不使用者應註冊裝置。
    
- 在 Azure 的入口網站移至**Intune\>裝置規範**。**監視**下按一下 [**裝置規範**。檢視裝置規範報告來驗證使用者的裝置標示為相容。 
    
- 在 Azure 的入口網站移至**Intune\>裝置規範**。在 [**管理**] 下按一下 [**原則**]。在規範遵守原則清單中，確認設定檔指派給使用者的裝置。如果沒有設定檔已指派，然後 Intune 將不能夠確認裝置的規範狀態。 
    
- 編輯使用者的設定格式化的條件存取工作分派。
    
1. 在 Azure 的入口網站移至**Intune\>條件式存取\>原則**
    
2. 從清單中選取的原則
    
3. 按一下 [**使用者與群組**
    
4. 若要將目標放在某個人的特定原則，請將其新增至**包含**清單中。若要確保人員省略從原則，請將其新增至**排除**清單中。 
    
閱讀更多：[如何監視設定格式化的條件存取裝置](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

