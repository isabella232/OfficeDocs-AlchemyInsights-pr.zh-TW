---
title: 設定格式化的條件 intune 的存取
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 3b50bc96a879017b62e42e1849f72e68408a0d9d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662318"
---
# <a name="conditional-access-with-intune"></a>設定格式化的條件 intune 的存取

使用**設定格式化的條件存取**intune 需要 3 個步驟： 
  
- 建立定義哪些資源所要受到保護，而需要存取這些資源符合的條件的**設定格式化的條件存取原則**。例如，裝置必須符合才存取公司的電子郵件。 
    
- 建立**規範原則**定義裝置會被視為相容前必須符合的設定。例如，裝置必須至少 6 位數的 pin 才會視為相容。 
    
- 確保**規範遵守原則**和**設定格式化的條件存取原則**會針對所需的使用者群組。這可能需要在 Azure Active Directory 中建立特定使用者群組。 
    
閱讀更多：
  
- [條件式存取的最佳作法](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [條件式存取的快速入門](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

