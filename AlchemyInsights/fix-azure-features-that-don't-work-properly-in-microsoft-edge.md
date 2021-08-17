---
title: 如果 Azure 功能在 Microsoft Edge 中無法正常運作，該怎麼辦
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004128"
- "7206"
ms.openlocfilehash: e188ecb375f3d84b45a1a7718b3c0b797c756f822ba64b3824976fe79c1e8298
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54117079"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a>如果 Azure 功能在 Microsoft Edge 中無法正常運作，該怎麼辦

Microsoft Edge 具有與安全性區域相關的[已知問題](https://go.microsoft.com/fwlink/?linkid=2140608)，而且可能會影響 Azure 使用者登入 Windows 系統管理中心的方式。 如果您在使用 Microsoft Edge Azure 功能時發生問題，請嘗試下列步驟：

1. 在 [ **開始** ] 功能表中，搜尋 [ **網際網路選項** ]，然後選取。
2. 在 [ **網際網路屬性** ] 對話方塊中，移至 [ **安全性** ] 索引標籤。
3. 選取 [ **信任的網站** ] 區域，然後選取 [ **網站** ] 按鈕。
4. 在 [ **信任的網站** ] 對話方塊中，新增您的閘道 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然後選取 [ **關閉**]。
5. 在 [ **網際網路屬性** ] 對話方塊中，移至 [ **隱私權** ] 索引標籤。
6. 在 [**彈出** 視窗封鎖程式] 區段中，選取 [**設定**]。 在開啟的對話方塊中，新增您的閘道 URL 以及 [https://login.microsoftonline.com](https://login.microsoftonline.com) 和 [https://login.live.com](https://login.live.com) ，然後選取 [ **關閉**]。
