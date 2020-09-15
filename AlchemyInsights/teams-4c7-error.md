---
title: 團隊4c7 錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700194"
---
# <a name="4c7-error-in-microsoft-teams"></a>Microsoft 小組中的4c7 錯誤

發生此錯誤的原因是 Microsoft 小組需要表單驗證。 當您部署 Active Directory Federation Services (AD FS) 時，預設不會啟用內部網路的表單驗證。 如果 Windows 整合式驗證失敗，系統會提示您使用表單驗證登入。

若要解決此問題，請在具有 Active Directory 本機複本的電腦上，使用 AD FS Microsoft Management Console (MMC) 嵌入式管理單元來啟用表單驗證。 如果要執行這項操作，請依照下列步驟執行： 

1. 在功能窗格中，流覽至 **驗證原則**。
2. 在詳細資料窗格的 [ **動作** ] 下，選取 [ **編輯全域主要驗證**]。
3. 在 [ **內部** 網路] 索引標籤上，選取 [ **表單驗證**]。
4. 選取 **[確定** (**Apply** ] 或 [套用) ]。