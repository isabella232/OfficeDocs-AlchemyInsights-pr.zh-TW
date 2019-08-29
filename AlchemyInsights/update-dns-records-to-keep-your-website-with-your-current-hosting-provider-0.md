---
title: 更新 DNS 記錄以便向目前的主機服務提供者保留網站
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665751"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="976d7-102">更新 DNS 記錄以便向目前的主機服務提供者保留網站</span><span class="sxs-lookup"><span data-stu-id="976d7-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="976d7-103">在 Microsoft 365 系統管理中心，移至 [**設定** > [網域](https://portal.office.com/adminportal/home#/Domains)] 頁面上，然後在 [網域] 清單中選取您對您的網站使用的網域。</span><span class="sxs-lookup"><span data-stu-id="976d7-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="976d7-104">選取 [ **+ 新增自訂記錄**，並輸入下列項目：</span><span class="sxs-lookup"><span data-stu-id="976d7-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="976d7-105">針對 [ **DNS 類型**]，輸入： **A （位址）**</span><span class="sxs-lookup"><span data-stu-id="976d7-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="976d7-106">**主機名稱或別名**，請輸入下列命令：**@**</span><span class="sxs-lookup"><span data-stu-id="976d7-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="976d7-107">**IP 位址**] 中，輸入您它目前主控 （例如，172.16.140.1） 的網站的靜態 IP 位址。</span><span class="sxs-lookup"><span data-stu-id="976d7-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="976d7-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span><span class="sxs-lookup"><span data-stu-id="976d7-p101">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="976d7-110">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="976d7-110">Select **Save**.</span></span>

<span data-ttu-id="976d7-111">此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。</span><span class="sxs-lookup"><span data-stu-id="976d7-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="976d7-112">選取 [ **+ 新增自訂記錄**，並輸入下列項目：</span><span class="sxs-lookup"><span data-stu-id="976d7-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="976d7-113">針對 [ **DNS 類型**]，輸入： **CNAME （別名）**</span><span class="sxs-lookup"><span data-stu-id="976d7-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="976d7-114">**主機名稱或別名**，請輸入下列命令： **www**</span><span class="sxs-lookup"><span data-stu-id="976d7-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="976d7-115">**指向位址**，輸入您的網站 (例如，contoso.com) 的完整的網域名稱 (FQDN)。</span><span class="sxs-lookup"><span data-stu-id="976d7-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="976d7-116">選取**儲存**。</span><span class="sxs-lookup"><span data-stu-id="976d7-116">Select **Save**.</span></span>
