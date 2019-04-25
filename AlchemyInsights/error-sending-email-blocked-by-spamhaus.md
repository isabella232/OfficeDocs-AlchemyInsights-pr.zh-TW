---
title: 傳送電子郵件遭到 SpamHaus 時發生錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402250"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>傳送電子郵件時發生錯誤： 使用 Spamhaus 封鎖的用戶端主機

傳送郵件的 IP 位址是由[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)擁有在封鎖清單上。 針對由 Spamhaus 遭到封鎖的原因包括遭入侵的帳戶，危害機器共用公用 IP 位址和網際網路服務提供者 (ISP) 原則。 可能的修正方法是：
  
- 您用來控制的來源電子郵件伺服器的 Office 365 封鎖接收傳入的郵件，您需要判定其原因及封鎖移除 Spamhaus 網站。
    
- 來源 IP 位址給其他人所屬的位置的 Office 365 封鎖接收傳入的郵件，地址擁有者必須從 Spamhaus 網站移除區塊。 原則封鎖清單 (PBL) 上的 IP 位址時，擁有者可以指派不同的靜態 IP 位址，或從 PBL 移除地址。
    
- 封鎖從您的 Office 365 網域的輸出郵件，您可以在如果郵件會路由傳送到 3rd 廠商服務收到此錯誤。 您可以使用 WHOIS 查閱工具以找出封鎖的 IP 位址擁有者。
    

