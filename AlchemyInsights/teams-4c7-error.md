---
title: Teams 4c7 錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: ea3e8f23c07103e604fc6b264047582b9c3e26b6b73237adc30eba574e06cfd3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54049299"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams 中的4c7 錯誤

發生此錯誤的原因是 Microsoft Teams 需要表單驗證。 當您部署 Active Directory Federation Services (AD FS) 時，預設不會啟用內部網路的表單驗證。 如果 Windows 整合驗證失敗，系統會提示您使用表單驗證登入。

若要解決此問題，請在具有 Active Directory 本機複本的電腦上，使用 AD FS Microsoft Management Console (MMC) 嵌入式管理單元來啟用表單驗證。 如果要執行這項操作，請依照下列步驟執行： 

1. 在功能窗格中，流覽至 **驗證原則**。
2. 在詳細資料窗格的 [ **動作** ] 下，選取 [ **編輯全域主要驗證**]。
3. 在 [ **內部** 網路] 索引標籤上，選取 [ **表單驗證**]。
4. 選取 **[確定** ( ] 或 [套用) ]。