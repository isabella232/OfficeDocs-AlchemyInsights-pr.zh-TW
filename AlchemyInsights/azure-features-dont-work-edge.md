---
title: 如果 Azure 功能在 Microsoft Edge 中無法正常運作，該怎麼辦
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8315"
- "9004429"
ms.openlocfilehash: 710489bd7dcb10f5c953c83e87bdad030c47cfda7dbd38e1eceae78bfe0d8790
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950321"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>如果 Azure 功能在 Microsoft Edge 中無法正常運作，該怎麼辦

Microsoft Edge 有與安全性區域相關的已知問題，可能會影響 Azure 使用者登入 Windows 系統管理中心的方式。 如需相關資訊，請參閱 [Edge 的已知問題](https://go.microsoft.com/fwlink/?linkid=2140608)。 如果您無法將 Azure 功能與 Microsoft Edge 一起使用，請嘗試下列方法：

1. 在 [開始] 功能表的 **[搜尋]** 列中，輸入 **網際網路選項**，然後選取它。
1. 在 **[網際網路內容]** 中，選取 **[安全性]** 索引標籤。
1. 選取 **[信任的網站]**，然後選取 **[網站]**。
1. 新增您的閘道 URL，以及 <https://login.microsoftonline.com> 和 <https://login.live.com>，然後選取 **[關閉]**。
1. 在 **[網際網路內容]** 中，選取 **[隱私權]** 索引標籤。
1. 在快顯視窗封鎖程式區段，選取 **[設定]**。 新增您的閘道 URL，以及 <https://login.microsoftonline.com> 和 <https://login.live.com>，然後選取 **[關閉]**。