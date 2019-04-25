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
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 [[網域](https://portal.office.com/adminportal/home#/Domains)] 頁面清單中的網域] 中，選取您正在使用您的網站，，然後選取 [管理] 窗格中的 [ **DNS 設定**的網域。 
    
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
    

