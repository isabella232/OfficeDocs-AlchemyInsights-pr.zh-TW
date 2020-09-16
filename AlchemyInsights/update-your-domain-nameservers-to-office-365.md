---
title: 將您的網域名稱伺服器更新為指向 Microsoft
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 7322fa640f6d043f057c8b7a5e06a18dcd10eec5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734902"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="c692a-102">將您的網域名稱伺服器更新為指向 Microsoft</span><span class="sxs-lookup"><span data-stu-id="c692a-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="c692a-103">附註：名稱伺服器變更最多可能需要 48 小時才會傳播。</span><span class="sxs-lookup"><span data-stu-id="c692a-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="c692a-104">若要使用 Microsoft 設定您的網域，必須更新您的註冊機上的名稱伺服器。</span><span class="sxs-lookup"><span data-stu-id="c692a-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="c692a-105">在網域註冊機構建立或編輯網域名稱伺服器記錄。</span><span class="sxs-lookup"><span data-stu-id="c692a-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="c692a-106">移至您的網域註冊機構網站，並找到可編輯名稱伺服器的區域。</span><span class="sxs-lookup"><span data-stu-id="c692a-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="c692a-107">建立或編輯兩項名稱伺服器以符合這些值：</span><span class="sxs-lookup"><span data-stu-id="c692a-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="c692a-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c692a-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="c692a-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="c692a-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="c692a-110">儲存變更。</span><span class="sxs-lookup"><span data-stu-id="c692a-110">Save changes.</span></span>

<span data-ttu-id="c692a-111">您也可以在本文中找到詳細指示： [Change 名稱伺服器以設定 Microsoft 365 與任何網域註冊機構](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="c692a-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  