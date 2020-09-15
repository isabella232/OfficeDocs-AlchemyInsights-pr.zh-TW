---
title: 變更名稱伺服器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 07a0dd19a768dd2b97923f0ced566b69ca2d6ba7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47714679"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="606bc-102">將您的網域名稱伺服器更新為指向 Microsoft</span><span class="sxs-lookup"><span data-stu-id="606bc-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="606bc-103">附註：名稱伺服器變更最多可能需要 48 小時才會傳播。</span><span class="sxs-lookup"><span data-stu-id="606bc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="606bc-p101">若要在 Microsoft 365 中設定網域，請在您的註冊機構更新名稱伺服器。在網域註冊機構建立或編輯網域名稱伺服器記錄。</span><span class="sxs-lookup"><span data-stu-id="606bc-p101">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="606bc-106">移至您的網域註冊機構網站，並找到可編輯名稱伺服器的區域。</span><span class="sxs-lookup"><span data-stu-id="606bc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="606bc-107">建立或編輯兩項名稱伺服器以符合這些值：</span><span class="sxs-lookup"><span data-stu-id="606bc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="606bc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="606bc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="606bc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="606bc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="606bc-110">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="606bc-110">Save changes.</span></span>

<span data-ttu-id="606bc-111">您也可以在這篇文章中找到詳細指示：[使用任何網域註冊機構變更名稱伺服器](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="606bc-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  