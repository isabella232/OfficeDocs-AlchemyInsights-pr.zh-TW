---
title: 傳送電子郵件 SpamHaus 所封鎖的錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 249f16d057b0539d71dc514ac35df28ab78fa061
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29912339"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="89120-102">傳送電子郵件的錯誤： 使用 Spamhaus 封鎖的用戶端主機</span><span class="sxs-lookup"><span data-stu-id="89120-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="89120-p101">傳送訊息的 IP 位址是由[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)擁有在封鎖清單上。Spamhaus 所封鎖的原因包含洩漏的帳戶危害機器共用公用 IP 位址及網際網路服務提供者 (ISP) 原則。可能的修正包括：</span><span class="sxs-lookup"><span data-stu-id="89120-p101">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies. Possible fixes are:</span></span>
  
- <span data-ttu-id="89120-106">您用來控制來源電子郵件伺服器的 Office 365 的封鎖內送郵件，您需要決定原因及移除 Spamhaus 網站中的封鎖。</span><span class="sxs-lookup"><span data-stu-id="89120-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="89120-p102">封鎖內送郵件至 Office 365 來源 IP 位址給其他人所屬的位置的地址擁有者必須移除 Spamhaus 網站中的封鎖。如果原則封鎖清單 (PBL) 的 IP 位址，其擁有人可以指派不同的靜態 IP 位址或從 PBL 移除地址。</span><span class="sxs-lookup"><span data-stu-id="89120-p102">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website. If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="89120-p103">封鎖從您的 Office 365 網域的外寄郵件，您才能接收此錯誤訊息都透過 3rd 廠商服務。您可以使用 WHOIS 查閱工具來尋找封鎖的 IP 位址擁有者。</span><span class="sxs-lookup"><span data-stu-id="89120-p103">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service. You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

