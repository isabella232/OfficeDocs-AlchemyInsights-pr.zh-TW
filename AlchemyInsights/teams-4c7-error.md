---
title: Teams 4 c 7 錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795992"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft Teams 中的 4 c 7 錯誤

因為 Microsoft Teams 要求表單驗證，則會發生這個錯誤。 當您部署 Active Directory Federation Services (AD FS) 時，表單驗證未啟用內部網路的預設值。 如果 Windows 整合式驗證失敗，系統會提示您使用表單驗證登入。

若要解決此問題，在具有 Active Directory 的本機複本的電腦上使用 [AD FS Microsoft Management Console (MMC) 嵌入式管理單元啟用表單驗證。 若要這樣做，請執行下列步驟： 

1. 在功能窗格中，瀏覽至**驗證原則**。
2. 在詳細資料窗格中的**動作**] 下選取 [**編輯通用主要驗證**]。
3. 在 [**內部網路**] 索引標籤上選取 [**表單驗證**]。
4. 選取 **[確定]** （或**套用**）。