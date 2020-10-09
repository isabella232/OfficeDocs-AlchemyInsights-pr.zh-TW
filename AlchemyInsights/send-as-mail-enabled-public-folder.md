---
title: 在 EXO 中以啟用郵件功能的公用資料夾傳送
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 0765262c04571e7df139de993611fd6e67068c54
ms.sourcegitcommit: 45635cc7a6c36d6c7b5f78215ad32f2aa7e3aed0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/08/2020
ms.locfileid: "48394686"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="de258-102">SendAs 啟用郵件功能的公用資料夾</span><span class="sxs-lookup"><span data-stu-id="de258-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="de258-103">下列範例會將擁有郵件功能之公用資料夾 NewPF1 的「傳送為」許可權指派給使用者 Jason。</span><span class="sxs-lookup"><span data-stu-id="de258-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="de258-104">Add-RecipientPermission 身分識別 ' NewPF1 '-受信者「Jason」-AccessRights ' SendAs '</span><span class="sxs-lookup"><span data-stu-id="de258-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="de258-105">如需詳細的語法及參數資訊，請參閱 [指派給擁有郵件功能之公用資料夾的「傳送為」或「代理傳送」許可權](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)。</span><span class="sxs-lookup"><span data-stu-id="de258-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>
