---
title: ConsistencyGuid / sourceAnchor 行為
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498509"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor 行為

Azure AD Connect (版本 1.1.524.0 及之後) 現在以加速型 ConsistencyGuid 為 sourceAnchor 屬性使用。使用這項功能時, Azure AD 連線會同步處理規則來自動設定：
  
- 使用型 ConsistencyGuid sourceAnchor 屬性為使用者物件。Objectguid 資訊用於其他物件類型。
    
- 任何特定的內部部署 AD 使用者物件其型 ConsistencyGuid 屬性不是其 objectguid 資訊值回到型 ConsistencyGuid 屬性在內部部署 Active Directory 中填入、 Azure AD Connect 寫入數。已填入型 ConsistencyGuid 屬性後，Azure AD 連線再將物件匯出至 Azure AD。
    
 **附註：** 一次內部部署 AD 物件匯入 Azure AD 連線 （亦即匯入 AD 連接器空間和 Metaverse 至預估），就無法再變更其 sourceAnchor 值。若要指定 sourceAnchor 值授與內部部署 AD 物件、 設定其型 ConsistencyGuid 屬性，再匯入至 Azure AD 連線。 
  
如需有關 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列： [Azure AD 連線： 設計概念](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

