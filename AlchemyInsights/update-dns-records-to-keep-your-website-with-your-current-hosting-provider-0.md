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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 [網域] 頁面的網域清單中，選取您要用於網站的網域，然後選取管理窗格中的 [DNS 設定]。 
    
2. 選取 [+ 新的自訂記錄]，然後輸入下列內容： 
    
  - 針對 [DNS 類型]，輸入： A (位址)
    
  - 為**主機名稱或別名**，請輸入下列命令：**@**
    
  - 針對 [IP 位址]，輸入目前裝載您網站的靜態 IP 位址 (例如，172.16.140.1)。 
    
    這必須是*靜態*IP 位址的網站不是*動態*的 IP 位址。檢查與站台主控您的網站以確定您可以取得靜態 IP 位址的公用網站。 
    
3. 選取 **[儲存]**。 
    
此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [+ 新的自訂記錄]，然後輸入下列內容： 
    
  - 針對 [DNS 類型]，輸入： CNAME (別名)
    
  - 針對 [主機名稱或別名]，輸入： www
    
  - 針對 [指向位址]，輸入網站的完整網域名稱 (FQDN) (例如：contoso.com)。 
    
2. 選取 **[儲存]**。 
    

