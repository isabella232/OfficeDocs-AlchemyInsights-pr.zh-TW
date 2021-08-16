---
title: 錯誤 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002111"
---
# <a name="error-attributevaluemustbeunique"></a>錯誤： AttributeValueMustBeUnique

AttributeValueMustBeUnique 錯誤最常見的原因是兩個物件具有不同的 SourceAnchor (immutableId) 具有相同的 ProxyAddresses 和/或 UserPrincipalName 屬性值。 修正 AttributeValueMustBeUnique 錯誤：
  
1. 識別導致錯誤的重複 proxyAddresses、userPrincipalName 或其他屬性值。 此外，也請識別有兩個以上的 (或多個) 物件與衝突有關。 Azure AD 所產生的報告連線同步處理的健康情況，可協助您識別這兩個物件。
    
2. 識別哪個物件應該繼續具有重複的值，而不應該是哪個物件。
    
3. 從 object 中移除不應該具有該值的重複值。 請注意，您應該在來源所在的目錄中進行變更。 在某些情況下，您可能需要刪除其中一個存在衝突的物件。
    
4. 如果您在內部部署 AD 中進行變更，請讓 Azure AD 連線同步處理錯誤的變更，以進行修正。
    

