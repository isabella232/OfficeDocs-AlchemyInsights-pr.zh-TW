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
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816983"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="8a061-102">ConsistencyGuid/sourceAnchor 行為</span><span class="sxs-lookup"><span data-stu-id="8a061-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="8a061-103">Azure AD Connect (版本1.1.524.0 及之後) 現在有利於使用 ConsistencyGuid 做為 sourceAnchor 屬性。</span><span class="sxs-lookup"><span data-stu-id="8a061-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="8a061-104">使用此功能時，Azure AD Connect 會自動將同步處理規則設定為：</span><span class="sxs-lookup"><span data-stu-id="8a061-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="8a061-105">使用 ConsistencyGuid 做為使用者物件的 sourceAnchor 屬性。</span><span class="sxs-lookup"><span data-stu-id="8a061-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="8a061-106">使用的是其他物件類型的 ObjectGUID。</span><span class="sxs-lookup"><span data-stu-id="8a061-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="8a061-107">對於任何未填入 ConsistencyGuid 屬性的任何內部部署 AD 使用者物件，Azure AD Connect 會寫入其 objectGUID 值回內部部署 Active Directory 中的 ConsistencyGuid 屬性。</span><span class="sxs-lookup"><span data-stu-id="8a061-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="8a061-108">在填入 ConsistencyGuid 屬性之後，Azure AD Connect 便會將物件匯出至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="8a061-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="8a061-109">**附注：** 將內部部署 AD 物件匯入 Azure AD Connect (也就是說，匯入至 AD 連接器空間，並投影入元節) 後，就無法再變更它的 sourceAnchor 值。</span><span class="sxs-lookup"><span data-stu-id="8a061-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="8a061-110">若要指定特定內部部署 AD 物件的 sourceAnchor 值，請在將其匯入 Azure AD Connect 之前，先設定其 ConsistencyGuid 屬性。</span><span class="sxs-lookup"><span data-stu-id="8a061-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="8a061-111">如需 SourceAnchor 和 ConsistencyGuid 的詳細資訊，請參閱下列內容： [AZURE AD Connect：設計概念](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="8a061-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

