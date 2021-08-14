---
title: 關於 Yammer 系統管理員
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003221"
- "9714"
ms.openlocfilehash: a5d71f509b7006264b15549c7e8450d4ed7025b7dea3cfd80fe6f0fdf50b0b9c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989690"
---
# <a name="about-yammer-admins"></a>關於 Yammer 系統管理員

**網路系統管理員**

全域管理員會自動升級為 Yammer 網路中已驗證的系統管理員角色。 在下列情況下，此升級可能無法正確進行：

- 多個 Yammer 網路都存在，且系統管理員已登入錯誤的網路。 若要取得單一 Yammer 網路，需要進行[網路整合](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)。
- 使用 Azure PIM。 使用者可能不會提升為全域系統管理員足夠長的時間來進行升級。 對 Yammer 的後續更新可解決此問題，但最好是手動將使用者提升為全域管理員。
- Yammer 網路存在同步問題。 在此情況下，將需要支援要求才能進行進一步調查。

如需 Yammer 系統管理員角色的詳細資訊，請參閱[Manage Yammer admins](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-admins)。

**群組管理員**

群組管理員 Microsoft 365 連接的群組會與 Azure AD 中的群組成員資格同步處理。 若為大型群組，此同步處理可能需要較長的期限。
