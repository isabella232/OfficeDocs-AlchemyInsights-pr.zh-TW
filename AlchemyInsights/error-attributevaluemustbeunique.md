---
title: 錯誤 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30766015"
---
# <a name="error-attributevaluemustbeunique"></a>錯誤： AttributeValueMustBeUnique

AttributeValueMustBeUnique 錯誤的常見原因是兩個物件具有不同 SourceAnchor (immutableId) 有相同的值的 ProxyAddresses 及/或 UserPrincipalName 屬性。 若要修正 AttributeValueMustBeUnique 錯誤：
  
1. 找出重複的 proxyAddresses、 userPrincipalName 或造成錯誤的其他屬性值。 也會識別哪些兩個 （或多個） 物件相關的衝突。 Azure AD Connect Health 的同步處理所產生的報告可協助您找出兩個物件。
    
2. 識別哪些物件應繼續有重複的值，以及哪些物件不應。
    
3. 移除重複的值從不應有該值的物件。 請注意，您應該物件源自所在的目錄中進行的變更。 在某些情況下，您可能需要刪除其中一個發生衝突的物件。
    
4. 如果您在內部部署 AD 中進行變更，讓 Azure AD Connect 同步處理錯誤，以取得固定的變更。
    

