---
title: 902 （重複物件由於同步處理錯誤）
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: f576460547110e0e599a9062ae03f690792fe635
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29919863"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="2cb70-102">重複物件由於同步處理錯誤</span><span class="sxs-lookup"><span data-stu-id="2cb70-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="2cb70-103">您可能會收到下列錯誤訊息的其中一個目錄同步作業完成時：</span><span class="sxs-lookup"><span data-stu-id="2cb70-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>
  
- <span data-ttu-id="2cb70-104">無法更新此物件的 Microsoft Online Services 因為此物件相關聯的下列屬性的可能已經與您的本機目錄中的其他物件相關聯的值。</span><span class="sxs-lookup"><span data-stu-id="2cb70-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>
    
- <span data-ttu-id="2cb70-105">您的 Microsoft Online Services 目錄中已經存在具有相同的 proxy 地址的同步處理的物件。</span><span class="sxs-lookup"><span data-stu-id="2cb70-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>
    
- <span data-ttu-id="2cb70-106">無法更新此物件因為此物件相關聯的下列屬性的可能已經與您的本機目錄服務中的其他物件相關聯的值： UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="2cb70-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>
    
<span data-ttu-id="2cb70-107">若要找出並修正的問題，下載和執行[IdFix DirSync 錯誤補救工具](https://www.microsoft.com/download/details.aspx?id=36832)。</span><span class="sxs-lookup"><span data-stu-id="2cb70-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>
  
<span data-ttu-id="2cb70-108">如需詳細資訊，請參閱[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。</span><span class="sxs-lookup"><span data-stu-id="2cb70-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
  

