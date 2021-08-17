---
title: ConsistencyGuid/sourceAnchor 行為
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
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044331"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor 行為

Azure AD 連線 (版本1.1.524.0 及之後) 現在有利於使用 ConsistencyGuid 做為 sourceAnchor 屬性。 使用此功能時，Azure AD 連線會自動將同步處理規則設定為：
  
- 使用 ConsistencyGuid 做為使用者物件的 sourceAnchor 屬性。 使用的是其他物件類型的 ObjectGUID。
    
- 對於任何未填入 ConsistencyGuid 屬性的任何內部部署 AD 使用者物件，Azure AD 連線會將其 objectGUID 值寫入內部部署 Active Directory 中的 ConsistencyGuid 屬性。 在填入 ConsistencyGuid 屬性之後，Azure AD 連線然後將物件匯出至 Azure AD。
    
 **附注：** 將內部部署 AD 物件匯入 Azure AD 之後連線 (也就是說，匯入至 AD 連接器空間並投影入元節) ，您就無法再變更它的 sourceAnchor 值。 若要指定特定內部部署 AD 物件的 sourceAnchor 值，請先設定其 ConsistencyGuid 屬性，再將其匯入 Azure AD 連線。 
  
如需 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列內容： [AZURE AD 連線：設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

