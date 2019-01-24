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
ms.openlocfilehash: 59f1aefaeec3d655b2388b00e7d58a8c2338504b
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460964"
---
# <a name="conditional-access-with-intune"></a>設定格式化的條件 intune 的存取

使用**設定格式化的條件存取**intune 需要 3 個步驟： 
  
- 建立定義哪些資源所要受到保護，而需要存取這些資源符合的條件的**設定格式化的條件存取原則**。例如，裝置必須符合才存取公司的電子郵件。 
    
- 建立**規範原則**定義裝置會被視為相容前必須符合的設定。例如，裝置必須至少 6 位數的 pin 才會視為相容。 
    
- 確保**規範遵守原則**和**設定格式化的條件存取原則**會針對所需的使用者群組。這可能需要在 Azure Active Directory 中建立特定使用者群組。 
    
閱讀其他資訊
  
- [條件式存取的最佳作法](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/best-practices)
    
- [條件式存取的快速入門](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

