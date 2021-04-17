---
title: 更新 DNS 記錄以便向目前的主機服務提供者保留網站
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827500"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="35231-102">更新 DNS 記錄以便向目前的主機服務提供者保留網站</span><span class="sxs-lookup"><span data-stu-id="35231-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="35231-103">在 Microsoft 365 系統管理中心中，移至 [**安裝**  >  [網域](https://admin.microsoft.com/Adminportal#/Domains)] 頁面，然後在網域清單中，選取您要用於網站的網域。</span><span class="sxs-lookup"><span data-stu-id="35231-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="35231-104">選取 [ **+ 新的自訂記錄** ]，然後輸入下列內容：</span><span class="sxs-lookup"><span data-stu-id="35231-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="35231-105">針對 **DNS** 輸入： **(位址)**</span><span class="sxs-lookup"><span data-stu-id="35231-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="35231-106">針對 [ **主機名稱或別名**]，輸入下列專案： **@**</span><span class="sxs-lookup"><span data-stu-id="35231-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="35231-107">在 [ **IP 位址**] 中，輸入目前主控 (之網站的靜態 IP 位址（例如，172.16.140.1) ）。</span><span class="sxs-lookup"><span data-stu-id="35231-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="35231-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span><span class="sxs-lookup"><span data-stu-id="35231-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="35231-110">選取 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="35231-110">Select **Save**.</span></span>

<span data-ttu-id="35231-111">此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。</span><span class="sxs-lookup"><span data-stu-id="35231-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="35231-112">選取 [ **+ 新的自訂記錄** ]，然後輸入下列內容：</span><span class="sxs-lookup"><span data-stu-id="35231-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="35231-113">針對 **DNS 類型** 輸入： **CNAME (別名)**</span><span class="sxs-lookup"><span data-stu-id="35231-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="35231-114">針對 [ **主機名稱或別名**]，輸入下列： **www**</span><span class="sxs-lookup"><span data-stu-id="35231-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="35231-115">在 [ **指向位址**] 中，為您的網站輸入完整功能變數名稱 (FQDN)  (例如，contoso.com) 。</span><span class="sxs-lookup"><span data-stu-id="35231-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="35231-116">選取 [儲存]。</span><span class="sxs-lookup"><span data-stu-id="35231-116">Select **Save**.</span></span>
