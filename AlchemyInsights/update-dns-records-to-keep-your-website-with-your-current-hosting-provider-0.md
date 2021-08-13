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
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007673"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 Microsoft 365 系統管理中心中，移至 [**安裝**  >  [網域](https://admin.microsoft.com/Adminportal#/Domains)] 頁面，然後在網域清單中，選取您要用於網站的網域。

2. 選取 [ **+ 新的自訂記錄** ]，然後輸入下列內容：

  - 針對 **DNS** 輸入： **(位址)**

  - 針對 [ **主機名稱或別名**]，輸入下列專案： **@**

  - 在 [ **IP 位址**] 中，輸入目前主控 (之網站的靜態 IP 位址（例如，172.16.140.1) ）。

    This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.

3. 選取 **[儲存]**。

此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [ **+ 新的自訂記錄** ]，然後輸入下列內容：

  - 針對 **DNS 類型** 輸入： **CNAME (別名)**

  - 針對 [ **主機名稱或別名**]，輸入下列： **www**

  - 在 [ **指向位址**] 中，為您的網站輸入完整功能變數名稱 (FQDN)  (例如，contoso.com) 。

2. 選取 [儲存]。
