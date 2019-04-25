---
title: 902 （因為重複物件的 sync 常見錯誤）
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 5/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: ce7eeb07cfde16e6d6856a9369c042dcf4f05b63
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420856"
---
# <a name="sync-errors-due-to-duplicate-objects"></a><span data-ttu-id="212d7-102">重複的物件由於同步處理錯誤</span><span class="sxs-lookup"><span data-stu-id="212d7-102">Sync errors due to duplicate objects</span></span>

<span data-ttu-id="212d7-103">目錄同步處理完成時，您可能會收到下列其中一個下列錯誤訊息：</span><span class="sxs-lookup"><span data-stu-id="212d7-103">You might receive one of the following error messages when directory synchronization finishes:</span></span>

- <span data-ttu-id="212d7-104">無法更新此物件在 Microsoft Online Services，因為此物件相關聯的下列屬性有可能已在您的本機目錄中的另一個物件相關聯的值。</span><span class="sxs-lookup"><span data-stu-id="212d7-104">Unable to update this object in Microsoft Online Services because the following attributes associated with this object have values that may already be associated with another object in your local directory.</span></span>

- <span data-ttu-id="212d7-105">在您的 Microsoft Online Services 目錄中已經存在具有相同的 proxy 位址的同步處理的物件。</span><span class="sxs-lookup"><span data-stu-id="212d7-105">A synchronized object with the same proxy address already exists in your Microsoft Online Services directory.</span></span>

- <span data-ttu-id="212d7-106">無法更新此物件，因為此物件相關聯的下列屬性有可能已在您的本機目錄服務中的另一個物件相關聯的值： UserPrincipalName。</span><span class="sxs-lookup"><span data-stu-id="212d7-106">Unable to update this object because the following attributes associated with this object have values that may already be associated with another object in your local directory services: UserPrincipalName.</span></span>

<span data-ttu-id="212d7-107">若要找出並修正問題，下載並執行[IdFix DirSync 錯誤補救工具](https://www.microsoft.com/download/details.aspx?id=36832)。</span><span class="sxs-lookup"><span data-stu-id="212d7-107">To identify and fix the issue, download and run the [IdFix DirSync Error Remediation Tool](https://www.microsoft.com/download/details.aspx?id=36832).</span></span>

<span data-ttu-id="212d7-108">如需詳細資訊，請參閱 < <b0>KB2647098</b0>。</span><span class="sxs-lookup"><span data-stu-id="212d7-108">For more information, see [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o).</span></span>
