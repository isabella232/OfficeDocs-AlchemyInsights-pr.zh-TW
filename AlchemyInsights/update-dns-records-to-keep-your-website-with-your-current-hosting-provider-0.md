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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 Microsoft 365 系統管理中心，移至 [**設定** > [網域](https://portal.office.com/adminportal/home#/Domains)] 頁面上，然後在 [網域] 清單中選取您對您的網站使用的網域。

2. 選取 [ **+ 新增自訂記錄**，並輸入下列項目：

  - 針對 [ **DNS 類型**]，輸入： **A （位址）**

  - **主機名稱或別名**，請輸入下列命令：**@**

  - **IP 位址**] 中，輸入您它目前主控 （例如，172.16.140.1） 的網站的靜態 IP 位址。

    This must be a  *static*  IP address for the website, not a  *dynamic*  IP address. Check with site where your website is hosted to make sure you can get a static IP address for your public website.

3. 選取**儲存**。

此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [ **+ 新增自訂記錄**，並輸入下列項目：

  - 針對 [ **DNS 類型**]，輸入： **CNAME （別名）**

  - **主機名稱或別名**，請輸入下列命令： **www**

  - **指向位址**，輸入您的網站 (例如，contoso.com) 的完整的網域名稱 (FQDN)。

2. 選取**儲存**。
