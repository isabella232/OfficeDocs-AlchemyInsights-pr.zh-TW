---
title: 將您的網域名稱伺服器更新為 Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/18/2019
ms.locfileid: "36742160"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="3ed89-102">將您的網域名稱伺服器更新為 Office 365</span><span class="sxs-lookup"><span data-stu-id="3ed89-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="3ed89-103">附註：名稱伺服器變更最多可能需要 48 小時才會傳播。</span><span class="sxs-lookup"><span data-stu-id="3ed89-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3ed89-p101">若要在 Office 365 設定網域，請在您的註冊機構更新名稱伺服器。在網域註冊機構建立或編輯網域名稱伺服器記錄。</span><span class="sxs-lookup"><span data-stu-id="3ed89-p101">To set up your domain in Office 365, the nameservers at your registrar need to be updated. Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3ed89-106">移至您的網域註冊機構網站，並找到可編輯名稱伺服器的區域。</span><span class="sxs-lookup"><span data-stu-id="3ed89-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="3ed89-107">建立或編輯兩項名稱伺服器以符合這些值：</span><span class="sxs-lookup"><span data-stu-id="3ed89-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3ed89-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3ed89-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3ed89-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3ed89-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3ed89-110">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="3ed89-110">Save changes.</span></span>

<span data-ttu-id="3ed89-111">您也可以在這篇文章中找到詳細指示：[運用任何網域註冊機構變更名稱伺服器以設定 Office 365](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="3ed89-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  