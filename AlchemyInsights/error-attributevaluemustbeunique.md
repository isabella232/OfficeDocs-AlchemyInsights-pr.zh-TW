---
title: 錯誤 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: fa1fdb35f1af250bc98aa61c0e5111f1f1b8aac4
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703165"
---
# <a name="error-attributevaluemustbeunique"></a>錯誤： AttributeValueMustBeUnique

AttributeValueMustBeUnique 錯誤最常見的原因是兩個具有不同 SourceAnchor （immutableId）的物件具有相同的 ProxyAddresses 和/或 UserPrincipalName 屬性值。 修正 AttributeValueMustBeUnique 錯誤：
  
1. 識別導致錯誤的重複 proxyAddresses、userPrincipalName 或其他屬性值。 此外，請識別衝突中所涉及的兩個（或多個）物件。 Azure AD Connect Health 同步處理所產生的報告可協助您識別這兩個物件。
    
2. 識別哪個物件應該繼續具有重複的值，而不應該是哪個物件。
    
3. 從 object 中移除不應該具有該值的重複值。 請注意，您應該在來源所在的目錄中進行變更。 在某些情況下，您可能需要刪除其中一個存在衝突的物件。
    
4. 如果您在內部部署 AD 中進行變更，請讓 Azure AD Connect 同步處理錯誤的變更，以進行修正。
    

