---
title: 使用 Intune 的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32393532"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 的條件式存取

使用 Intune 使用**條件式存取**需要 3 個步驟： 
  
- 建立一個**條件式存取原則**來定義哪些資源會受到保護，以及條件必須符合要存取這些資源。 例如，裝置必須符合之前存取公司電子郵件。 
    
- 建立**符合性原則**來定義必須先符合裝置會被視為相容的設定。 例如，裝置必須至少 6 位數字的 pin 碼之前會被視為相容。 
    
- 確保**符合性原則**和**條件式存取原則**的目標的使用者所需的群組。 這可能需要在 Azure Active Directory 中建立特定使用者群組。 
    
深入了解：
  
- [條件式存取的最佳作法](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [開始使用條件式存取](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

