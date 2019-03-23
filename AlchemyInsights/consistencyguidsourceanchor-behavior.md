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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753093"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="fed79-102">ConsistencyGuid / sourceAnchor 行為</span><span class="sxs-lookup"><span data-stu-id="fed79-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="fed79-103">Azure AD Connect (版本 1.1.524.0 年) 現在可加速 Msds-alloweddnssuffixes ConsistencyGuid 做 sourceAnchor 屬性。</span><span class="sxs-lookup"><span data-stu-id="fed79-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="fed79-104">當使用這項功能，Azure AD Connect 會自動設定所要的同步處理規則：</span><span class="sxs-lookup"><span data-stu-id="fed79-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="fed79-105">作為 Msds-alloweddnssuffixes ConsistencyGuid sourceAnchor 屬性的 User 物件。</span><span class="sxs-lookup"><span data-stu-id="fed79-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="fed79-106">ObjectGUID 用於其他的物件類型。</span><span class="sxs-lookup"><span data-stu-id="fed79-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="fed79-107">任何給定的內部部署 AD 使用者其 Msds-alloweddnssuffixes ConsistencyGuid 屬性未填入、 Azure AD Connect 寫入其 objectGUID 值回內部部署 Active Directory 中的 Msds-alloweddnssuffixes ConsistencyGuid 屬性的物件。</span><span class="sxs-lookup"><span data-stu-id="fed79-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="fed79-108">填入 Msds-alloweddnssuffixes ConsistencyGuid 屬性後，Azure AD Connect 然後將物件匯出至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="fed79-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="fed79-109">**附註：** 一次內部部署 AD 物件匯入 Azure AD Connect （亦即匯入 AD 連接器空間和投影到 Metaverse），您無法再變更其 sourceAnchor 值。</span><span class="sxs-lookup"><span data-stu-id="fed79-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="fed79-110">若要指定 sourceAnchor 值指定內部部署 AD 物件、 設定其 Msds-alloweddnssuffixes ConsistencyGuid 屬性，再匯入到 Azure AD Connect。</span><span class="sxs-lookup"><span data-stu-id="fed79-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="fed79-111">如需有關 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列： [Azure AD Connect： 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="fed79-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

