---
title: Dynamics 365-Dynamics 365 統一介面中顯示錯誤的儀表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101473"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 統一介面中顯示錯誤的儀表板

您看到的儀表板可能與您預期的不同，原因如下：

## <a name="the-user-has-set-a-user-default-dashboard"></a>使用者已設定使用者預設儀表板 

一般來說，如果 [ **設定為預設** 值] 按鈕未顯示在儀表板命令列中，您可以識別使用者預設的儀表板。 使用者預設儀表板會覆寫所有其他的預設儀表板，即使使用者的預設儀表板不在目前的應用程式中也是一樣。

請使用下列解決方法來取消設置其預設儀表板。

1. 建立新的個人儀表板。

2. 將新的儀表板設定為使用者預設。

3. 刪除該儀表板。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>儀表板是在網站地圖中設定

您可以選取儀表板，然後選擇 [自訂系統] 底下的 [設為預設值]，以設定組織的預設儀表板。 不過，如果使用者可以存取，則在網站地圖設計工具中定義的儀表板會優先于此儀表板。

若要讓使用者看到您已設定為組織預設的儀表板，您可以執行下列其中一項操作：

* 在網站地圖中設定該儀表板

* 移除對那些使用者的網站地圖定義儀表板的存取權
