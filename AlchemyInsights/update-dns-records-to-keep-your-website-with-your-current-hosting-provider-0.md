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
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 62f49038cf541c2185ed6a60c6cb58fe2889342d
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353168"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="bba33-102">更新 DNS 記錄以便向目前的主機服務提供者保留網站</span><span class="sxs-lookup"><span data-stu-id="bba33-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="bba33-103">在 [[網域](https://portal.office.com/adminportal/home#/Domains)] 頁面上的網域清單中, 選取您要用於網站的網域, 然後選取 [管理] 窗格中的 [ **DNS 設定**]。</span><span class="sxs-lookup"><span data-stu-id="bba33-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website, and then select **DNS settings** in the management pane.</span></span>

2. <span data-ttu-id="bba33-104">選取 [ **+ 新的自訂記錄**], 然後輸入下列內容:</span><span class="sxs-lookup"><span data-stu-id="bba33-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bba33-105">針對 [ **DNS 類型**], 輸入: **A (位址)**</span><span class="sxs-lookup"><span data-stu-id="bba33-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="bba33-106">針對 [**主機名稱或別名**], 輸入下列專案:**@**</span><span class="sxs-lookup"><span data-stu-id="bba33-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="bba33-107">在 [ **IP 位址**] 中, 輸入目前所主控網站的靜態 IP 位址 (例如, 172.16.140.1)。</span><span class="sxs-lookup"><span data-stu-id="bba33-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="bba33-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span><span class="sxs-lookup"><span data-stu-id="bba33-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="bba33-110">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="bba33-110">Select **Save**.</span></span>

<span data-ttu-id="bba33-111">此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。</span><span class="sxs-lookup"><span data-stu-id="bba33-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="bba33-112">選取 [ **+ 新的自訂記錄**], 然後輸入下列內容:</span><span class="sxs-lookup"><span data-stu-id="bba33-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="bba33-113">針對 [ **DNS 類型**], 輸入: **CNAME (別名)**</span><span class="sxs-lookup"><span data-stu-id="bba33-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="bba33-114">針對 [**主機名稱或別名**], 輸入下列內容: **www**</span><span class="sxs-lookup"><span data-stu-id="bba33-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="bba33-115">針對 [**指向位址**], 輸入您網站的完整功能變數名稱 (FQDN) (例如, contoso.com)。</span><span class="sxs-lookup"><span data-stu-id="bba33-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="bba33-116">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="bba33-116">Select **Save**.</span></span>
