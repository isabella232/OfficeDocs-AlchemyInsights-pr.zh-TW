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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="2f0fd-102">傳送電子郵件時出錯: 已使用 Spamhaus 封鎖用戶端主機</span><span class="sxs-lookup"><span data-stu-id="2f0fd-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="2f0fd-103">傳送郵件的 IP 位址位於[Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)所擁有的封鎖清單上。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="2f0fd-104">Spamhaus 封鎖的原因包括受到影響的帳戶、共用公用 IP 位址的受害機器, 以及網際網路服務提供者 (ISP) 原則。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="2f0fd-105">可能的修正包括:</span><span class="sxs-lookup"><span data-stu-id="2f0fd-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="2f0fd-106">若要在您控制來源電子郵件伺服器的情況下, 將封鎖的內送郵件傳送至 Office 365, 您必須判斷原因並從 Spamhaus 網站移除區塊。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="2f0fd-107">針對已封鎖的輸入郵件至 Office 365, 其中來源 IP 位址隸屬于其他人, 位址擁有者必須從 Spamhaus 網站移除該區塊。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="2f0fd-108">如果 IP 位址位於原則封鎖清單 (PBL), 則擁有者可以指派不同的靜態 IP 位址, 或從 PBL 中移除位址。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="2f0fd-109">若要防止來自您 Office 365 網域的輸出郵件, 如果郵件是透過協力廠商服務路由傳送, 您就可以收到此錯誤。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="2f0fd-110">您可以使用 WHOIS 查閱工具來尋找封鎖的 IP 位址擁有者。</span><span class="sxs-lookup"><span data-stu-id="2f0fd-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
