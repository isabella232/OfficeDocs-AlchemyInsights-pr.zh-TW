---
title: 傳送 SpamHaus 封鎖的電子郵件時發生錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 52a5c20d59a2eac4c4bf465edaa888952d47f39f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387840"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>傳送電子郵件時出錯: 已使用 Spamhaus 封鎖用戶端主機

傳送郵件的 IP 位址位於[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)所擁有的封鎖清單上。 Spamhaus 封鎖的原因包括受到影響的帳戶、共用公用 IP 位址的受害機器, 以及網際網路服務提供者 (ISP) 原則。 可能的修正包括:
  
- 若要在您控制來源電子郵件伺服器的情況下, 將封鎖的內送郵件傳送至 Office 365, 您必須判斷原因並從 Spamhaus 網站移除區塊。

- 針對已封鎖的輸入郵件至 Office 365, 其中來源 IP 位址隸屬于其他人, 位址擁有者必須從 Spamhaus 網站移除該區塊。 如果 IP 位址位於原則封鎖清單 (PBL), 則擁有者可以指派不同的靜態 IP 位址, 或從 PBL 中移除位址。

- 若要防止來自您 Office 365 網域的輸出郵件, 如果郵件是透過協力廠商服務路由傳送, 您就可以收到此錯誤。 您可以使用 WHOIS 查閱工具來尋找封鎖的 IP 位址擁有者。
