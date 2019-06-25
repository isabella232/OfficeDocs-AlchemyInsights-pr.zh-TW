---
title: 902 (由於重複的物件而造成的同步處理錯誤)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 06cd582c30a59a94ee117728bd5daebecca77bc8
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757986"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="545db-102">由於重複的物件而造成的同步處理錯誤</span><span class="sxs-lookup"><span data-stu-id="545db-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="545db-103">目錄同步處理完成時, 您可能會收到下列其中一則錯誤訊息:</span><span class="sxs-lookup"><span data-stu-id="545db-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="545db-104">無法在 Microsoft Online Services 中更新此物件, 因為與此物件相關聯的下列屬性的值可能已經與您的本機目錄中的另一個物件相關聯。</span><span class="sxs-lookup"><span data-stu-id="545db-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="545db-105">您的 Microsoft Online Services 目錄中已存在具有相同 proxy 位址的已同步處理物件。</span><span class="sxs-lookup"><span data-stu-id="545db-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="545db-106">無法更新此物件, 因為與此物件相關聯的下列屬性的值可能已經與您的本機目錄服務: UserPrincipalName 中的另一個物件相關聯。</span><span class="sxs-lookup"><span data-stu-id="545db-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="545db-107">若要識別並修正問題, 請下載並執行[IdFix DirSync 錯誤修復工具](https://www.microsoft.com/download/details.aspx?id=36832)。</span><span class="sxs-lookup"><span data-stu-id="545db-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="545db-108">如需詳細資訊, 請參閱[KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。</span><span class="sxs-lookup"><span data-stu-id="545db-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
