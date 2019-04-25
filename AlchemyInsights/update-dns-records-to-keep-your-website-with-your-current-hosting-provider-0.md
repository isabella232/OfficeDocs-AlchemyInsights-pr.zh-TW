---
title: 更新 DNS 記錄以便向目前的主機服務提供者保留網站
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f2cdb319e56b82c09b7a9856c81a45e69dee6759
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32423714"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="28e53-102">更新 DNS 記錄以便向目前的主機服務提供者保留網站</span><span class="sxs-lookup"><span data-stu-id="28e53-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="28e53-103">在 [[網域](https://portal.office.com/adminportal/home#/Domains)] 頁面清單中的網域] 中，選取您正在使用您的網站，，然後選取 [管理] 窗格中的 [ **DNS 設定**的網域。</span><span class="sxs-lookup"><span data-stu-id="28e53-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span> 
    
2. <span data-ttu-id="28e53-104">選取 [ **+ 新增自訂記錄**，並輸入下列項目：</span><span class="sxs-lookup"><span data-stu-id="28e53-104">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="28e53-105">針對 [ **DNS 類型**]，輸入： **A （位址）**</span><span class="sxs-lookup"><span data-stu-id="28e53-105">For **DNS type** enter: **A (Address)**</span></span>
    
  - <span data-ttu-id="28e53-106">**主機名稱或別名**，請輸入下列命令：**@**</span><span class="sxs-lookup"><span data-stu-id="28e53-106">For **Host name or Alias**, type the following: **@**</span></span>
    
  - <span data-ttu-id="28e53-107">**IP 位址**] 中，輸入您它目前主控 （例如，172.16.140.1） 的網站的靜態 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="28e53-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span> 
    
    <span data-ttu-id="28e53-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span><span class="sxs-lookup"><span data-stu-id="28e53-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span> 
    
3. <span data-ttu-id="28e53-110">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="28e53-110">Select **Save**.</span></span> 
    
<span data-ttu-id="28e53-111">此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。</span><span class="sxs-lookup"><span data-stu-id="28e53-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="28e53-112">選取 [ **+ 新增自訂記錄**，並輸入下列項目：</span><span class="sxs-lookup"><span data-stu-id="28e53-112">Select **+ New custom record** and enter the following:</span></span> 
    
  - <span data-ttu-id="28e53-113">針對 [ **DNS 類型**]，輸入： **CNAME （別名）**</span><span class="sxs-lookup"><span data-stu-id="28e53-113">For **DNS type** enter: **CNAME (Alias)**</span></span>
    
  - <span data-ttu-id="28e53-114">**主機名稱或別名**，請輸入下列命令： **www**</span><span class="sxs-lookup"><span data-stu-id="28e53-114">For **Host name or Alias**, type the following: **www**</span></span>
    
  - <span data-ttu-id="28e53-115">**指向位址**，輸入您的網站 (例如，contoso.com) 的完整的網域名稱 (FQDN)。</span><span class="sxs-lookup"><span data-stu-id="28e53-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span> 
    
2. <span data-ttu-id="28e53-116">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="28e53-116">Select **Save**.</span></span> 
    

