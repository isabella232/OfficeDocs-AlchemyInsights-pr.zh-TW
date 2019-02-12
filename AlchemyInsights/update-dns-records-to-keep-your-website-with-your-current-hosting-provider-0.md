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
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e0dadba1e3ffd1cf0d49c0a76ec2efbbc6ae92db
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29906111"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>更新 DNS 記錄以便向目前的主機服務提供者保留網站

1. 在 [[網域](https://portal.office.com/adminportal/home#/Domains)] 頁面上的網域清單中選取您使用您網站，然後選取 [管理] 窗格中的 [ **DNS 設定**的網域。 
    
2. 選取 [ **+ 新增自訂的記錄**，輸入下列項目： 
    
  - **DNS**類型輸入: **（位址）**
    
  - 為**主機名稱或別名**，請輸入下列命令：**@**
    
  - 針對**IP 位址**] 中，輸入其目前主控 （例如 172.16.140.1） 您網站的靜態 IP 位址。 
    
    這必須是*靜態*IP 位址的網站不是*動態*的 IP 位址。檢查與站台主控您的網站以確定您可以取得靜態 IP 位址的公用網站。 
    
3. 選取 **[儲存]**。 
    
此外，您還可以建立 CNAME 記錄，協助客戶找到您的網站。
  
1. 選取 [ **+ 新增自訂的記錄**，輸入下列項目： 
    
  - **DNS**類型輸入： **CNAME (Alias)**
    
  - 為**主機名稱或別名**，請輸入下列命令： **www**
    
  - **指向位址**，輸入您的網站 (例如 contoso.com) 的完整的網域名稱 (FQDN)。 
    
2. 選取 **[儲存]**。 
    

