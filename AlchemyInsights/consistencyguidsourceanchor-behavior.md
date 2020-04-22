---
title: ConsistencyGuid/sourceAnchor 行為
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705724"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor 行為

Azure AD Connect （版本1.1.524.0 及之後）現在有利於使用 ConsistencyGuid 做為 sourceAnchor 屬性。 使用此功能時，Azure AD Connect 會自動將同步處理規則設定為：
  
- 使用 ConsistencyGuid 做為使用者物件的 sourceAnchor 屬性。 使用的是其他物件類型的 ObjectGUID。
    
- 對於任何未填入 ConsistencyGuid 屬性的任何內部部署 AD 使用者物件，Azure AD Connect 會寫入其 objectGUID 值回內部部署 Active Directory 中的 ConsistencyGuid 屬性。 在填入 ConsistencyGuid 屬性之後，Azure AD Connect 便會將物件匯出至 Azure AD。
    
 **附注：** 將內部部署 AD 物件匯入 Azure AD Connect （也就是匯入 AD 連接器空間並投影入元節）之後，就無法再變更它的 sourceAnchor 值。 若要指定特定內部部署 AD 物件的 sourceAnchor 值，請在將其匯入 Azure AD Connect 之前，先設定其 ConsistencyGuid 屬性。 
  
如需 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列內容： [AZURE AD Connect：設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

