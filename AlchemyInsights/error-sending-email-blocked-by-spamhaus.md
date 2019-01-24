---
title: 傳送電子郵件 SpamHaus 所封鎖的錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460381"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>傳送電子郵件的錯誤： 使用 Spamhaus 封鎖的用戶端主機

傳送訊息的 IP 位址是由[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)擁有在封鎖清單上。Spamhaus 所封鎖的原因包含洩漏的帳戶危害機器共用公用 IP 位址及網際網路服務提供者 (ISP) 原則。可能的修正包括：
  
- 您用來控制來源電子郵件伺服器的 Office 365 的封鎖內送郵件，您需要決定原因及移除 Spamhaus 網站中的封鎖。
    
- 封鎖內送郵件至 Office 365 來源 IP 位址給其他人所屬的位置的地址擁有者必須移除 Spamhaus 網站中的封鎖。如果原則封鎖清單 (PBL) 的 IP 位址，其擁有人可以指派不同的靜態 IP 位址或從 PBL 移除地址。
    
- 封鎖從您的 Office 365 網域的外寄郵件，您才能接收此錯誤訊息都透過 3rd 廠商服務。您可以使用 WHOIS 查閱工具來尋找封鎖的 IP 位址擁有者。
    

