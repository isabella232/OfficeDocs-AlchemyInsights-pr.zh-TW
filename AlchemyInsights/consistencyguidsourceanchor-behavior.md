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
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659582"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="f198e-102">ConsistencyGuid / sourceAnchor 行為</span><span class="sxs-lookup"><span data-stu-id="f198e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="f198e-p101">Azure AD Connect (版本 1.1.524.0 及之後) 現在以加速型 ConsistencyGuid 為 sourceAnchor 屬性使用。使用這項功能時, Azure AD 連線會同步處理規則來自動設定：</span><span class="sxs-lookup"><span data-stu-id="f198e-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="f198e-p102">使用型 ConsistencyGuid sourceAnchor 屬性為使用者物件。Objectguid 資訊用於其他物件類型。</span><span class="sxs-lookup"><span data-stu-id="f198e-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="f198e-p103">任何特定的內部部署 AD 使用者物件其型 ConsistencyGuid 屬性不是其 objectguid 資訊值回到型 ConsistencyGuid 屬性在內部部署 Active Directory 中填入、 Azure AD Connect 寫入數。已填入型 ConsistencyGuid 屬性後，Azure AD 連線再將物件匯出至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="f198e-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="f198e-p104">**附註：** 一次內部部署 AD 物件匯入 Azure AD 連線 （亦即匯入 AD 連接器空間和 Metaverse 至預估），就無法再變更其 sourceAnchor 值。若要指定 sourceAnchor 值授與內部部署 AD 物件、 設定其型 ConsistencyGuid 屬性，再匯入至 Azure AD 連線。</span><span class="sxs-lookup"><span data-stu-id="f198e-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="f198e-111">如需有關 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列： [Azure AD 連線： 設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="f198e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

