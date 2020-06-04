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
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665751"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 Microsoft 365 系統管理中心中，移至 [**安裝**  >  [網域](https://portal.office.com/adminportal/home#/Domains)] 頁面，然後在網域清單中，選取您要用於網站的網域。

2. 選取 [ **+ 新的自訂記錄**]，然後輸入下列內容：

  - 針對**DNS**輸入： **A （位址）**

  - 針對 [**主機名稱或別名**]，輸入下列專案：**@**

  - 在 [ **IP 位址**] 中，輸入目前所主控之網站的靜態 IP 位址（例如，172.16.140.1）。

    This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.

3. 選取 **[儲存]**。

此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [ **+ 新的自訂記錄**]，然後輸入下列內容：

  - 針對**DNS 類型**輸入： **CNAME （別名）**

  - 針對 [**主機名稱或別名**]，輸入下列： **www**

  - 在 [**指向位址**] 中，輸入您網站的完整功能變數名稱（FQDN）（例如，contoso.com）。

2. 選取 [儲存]****。
