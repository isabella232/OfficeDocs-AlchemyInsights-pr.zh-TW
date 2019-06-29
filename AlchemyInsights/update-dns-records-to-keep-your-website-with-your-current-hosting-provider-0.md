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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 [[網域](https://portal.office.com/adminportal/home#/Domains)] 頁面上的網域清單中, 選取您要用於網站的網域, 然後選取 [管理] 窗格中的 [ **DNS 設定**]。

2. 選取 [ **+ 新的自訂記錄**], 然後輸入下列內容:

  - 針對 [ **DNS 類型**], 輸入: **A (位址)**

  - 針對 [**主機名稱或別名**], 輸入下列專案:**@**

  - 在 [ **IP 位址**] 中, 輸入目前所主控網站的靜態 IP 位址 (例如, 172.16.140.1)。

    This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.

3. 選取**儲存**。

此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [ **+ 新的自訂記錄**], 然後輸入下列內容:

  - 針對 [ **DNS 類型**], 輸入: **CNAME (別名)**

  - 針對 [**主機名稱或別名**], 輸入下列內容: **www**

  - 針對 [**指向位址**], 輸入您網站的完整功能變數名稱 (FQDN) (例如, contoso.com)。

2. 選取**儲存**。
