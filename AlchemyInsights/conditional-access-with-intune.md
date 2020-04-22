---
title: 使用 Intune 的條件式存取
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706012"
---
# <a name="conditional-access-with-intune"></a>使用 Intune 的條件式存取

使用具有 Intune 的**條件式存取**需要三個步驟： 
  
- 建立**條件式存取原則**，以定義要保護的資源，以及存取這些資源所需符合的條件。 例如，裝置必須先相容才能存取公司的電子郵件。 
    
- 建立**相容性原則**，以定義在將裝置視為合規性之前必須滿足的設定。 例如，裝置的 pin 碼至少必須是6位數，才會被視為相容。 
    
- 確保**相容性原則**和**條件式存取原則**都是以所需的使用者群組為目標。 這可能需要在 Azure Active Directory 中建立特定的使用者群組。 
    
閱讀其他資訊：
  
- [條件式存取的最佳作法](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [條件式存取快速入門](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

