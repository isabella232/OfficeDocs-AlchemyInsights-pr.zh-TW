---
title: 更新 DNS 記錄以便向目前的主機服務提供者保留網站
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
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460594"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="af0db-102">更新 DNS 記錄以便向目前的主機服務提供者保留網站</span><span class="sxs-lookup"><span data-stu-id="af0db-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="af0db-103">在 [網域] 頁面的網域清單中，選取您要用於網站的網域，然後選取管理窗格中的 [DNS 設定]。</span><span class="sxs-lookup"><span data-stu-id="af0db-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="af0db-104">選取 [+ 新的自訂記錄]，然後輸入下列內容：</span><span class="sxs-lookup"><span data-stu-id="af0db-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="af0db-105">針對 [DNS 類型]，輸入： A (位址)</span><span class="sxs-lookup"><span data-stu-id="af0db-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="af0db-106">為**主機名稱或別名**，請輸入下列命令：**@**</span><span class="sxs-lookup"><span data-stu-id="af0db-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="af0db-107">針對 [IP 位址]，輸入目前裝載您網站的靜態 IP 位址 (例如，172.16.140.1)。</span><span class="sxs-lookup"><span data-stu-id="af0db-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="af0db-p101">這必須是*靜態*IP 位址的網站不是*動態*的 IP 位址。檢查與站台主控您的網站以確定您可以取得靜態 IP 位址的公用網站。</span><span class="sxs-lookup"><span data-stu-id="af0db-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="af0db-110">選取 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="af0db-110">Select **Save**.</span></span> 
    
<span data-ttu-id="af0db-111">此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。</span><span class="sxs-lookup"><span data-stu-id="af0db-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="af0db-112">選取 [+ 新的自訂記錄]，然後輸入下列內容：</span><span class="sxs-lookup"><span data-stu-id="af0db-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="af0db-113">針對 [DNS 類型]，輸入： CNAME (別名)</span><span class="sxs-lookup"><span data-stu-id="af0db-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="af0db-114">針對 [主機名稱或別名]，輸入： www</span><span class="sxs-lookup"><span data-stu-id="af0db-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="af0db-115">針對 [指向位址]，輸入網站的完整網域名稱 (FQDN) (例如：contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="af0db-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="af0db-116">選取 **[儲存]**。</span><span class="sxs-lookup"><span data-stu-id="af0db-116">Select **Save**.</span></span> 
    

