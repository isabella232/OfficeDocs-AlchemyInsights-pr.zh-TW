---
title: ConsistencyGuid / sourceAnchor 行為
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516963"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor 行為

Azure AD Connect (版本 1.1.524.0 年) 現在可加速 Msds-alloweddnssuffixes ConsistencyGuid 做 sourceAnchor 屬性。 當使用這項功能，Azure AD Connect 會自動設定所要的同步處理規則：
  
- 作為 Msds-alloweddnssuffixes ConsistencyGuid sourceAnchor 屬性的 User 物件。 ObjectGUID 用於其他的物件類型。
    
- 任何給定的內部部署 AD 使用者其 Msds-alloweddnssuffixes ConsistencyGuid 屬性未填入、 Azure AD Connect 寫入其 objectGUID 值回內部部署 Active Directory 中的 Msds-alloweddnssuffixes ConsistencyGuid 屬性的物件。 填入 Msds-alloweddnssuffixes ConsistencyGuid 屬性後，Azure AD Connect 然後將物件匯出至 Azure AD。
    
 **附註：** 一次內部部署 AD 物件匯入 Azure AD Connect （亦即匯入 AD 連接器空間和投影到 Metaverse），您無法再變更其 sourceAnchor 值。 若要指定 sourceAnchor 值指定內部部署 AD 物件、 設定其 Msds-alloweddnssuffixes ConsistencyGuid 屬性，再匯入到 Azure AD Connect。 
  
如需有關 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列： [Azure AD Connect： 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

