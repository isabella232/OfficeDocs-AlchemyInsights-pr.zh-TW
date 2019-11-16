---
title: Dynamics 365-Dynamics 365 整合介面中顯示錯誤的儀表板
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "36528542"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 整合介面中顯示錯誤的儀表板

有幾個理由為什麼您可能會看到比您預期不同儀表板：

## <a name="the-user-has-set-a-user-default-dashboard"></a>使用者已設定的使用者預設儀表板 

通常可以將使用者識別如果**設為預設值**] 按鈕不會顯示在儀表板命令列會設為預設儀表板。 使用者預設儀表板會覆寫所有其他預設儀表板，即使使用者的預設儀表板並不是在目前的應用程式中。

使用下列因應措施未設定其預設儀表板。

1. 建立新的個人儀表板。

2. 設定新儀表板的使用者預設值。

3. 刪除儀表板。

## <a name="the-dashboard-is-set-in-the-sitemap"></a>在網站地圖中設定儀表板

您可以藉由選取儀表板，然後選擇 [設成預設值 '' 自訂系統 '] 下將設定組織預設儀表板。 但在網站地圖設計工具中定義的儀表板將優先於此儀表板，如果使用者具有其存取權。

若要讓使用者看到您已設定為組織預設儀表板，您可以：

* 在網站地圖中設定儀表板

* 移除這些使用者定義的網站地圖儀表板的存取
