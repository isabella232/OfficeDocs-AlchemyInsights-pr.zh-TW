---
title: 錯誤 AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7a97d1a5ff352b55833bd457e3220a56130d7e7e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499625"
---
# <a name="error-attributevaluemustbeunique"></a>錯誤： AttributeValueMustBeUnique

AttributeValueMustBeUnique 錯誤的最常見原因是兩個物件具有不同 SourceAnchor (immutableId) 具有相同 ProxyAddresses 和/或 UserPrincipalName 屬性的值。若要修正 AttributeValueMustBeUnique 錯誤：
  
1. 找出重複的 proxyAddresses、 userPrincipalName 或其他屬性值會導致錯誤。也會識別兩個 （或多個） 物件相關衝突。Azure AD 連線狀況的同步處理所產生的報告可協助您識別兩個物件。
    
2. 找出哪個物件應繼續有重複的值並不應該哪個物件。
    
3. 物件中不應有該值移除重複的值。請注意您應該會從聆聽來源物件的目錄中進行變更。在某些情況下，您可能需要刪除其中一個物件發生衝突。
    
4. 如果您在內部部署 AD 中做的變更，可讓 Azure AD 連線同步處理來取得修正錯誤的變更。
    

