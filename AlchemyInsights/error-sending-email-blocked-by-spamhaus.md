---
title: 傳送 SpamHaus 封鎖的電子郵件時發生錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813715"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="b5c8f-102">傳送電子郵件時出錯：已使用 Spamhaus 封鎖用戶端主機</span><span class="sxs-lookup"><span data-stu-id="b5c8f-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="b5c8f-103">傳送郵件的 IP 位址位於 [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245)所擁有的封鎖清單上。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="b5c8f-104">Spamhaus 封鎖的原因包括已遭破壞的帳戶、共用公用 IP 位址的受損機器，以及網際網路服務提供者 (ISP) 原則。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="b5c8f-105">可能的修正包括：</span><span class="sxs-lookup"><span data-stu-id="b5c8f-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="b5c8f-106">針對您控制來源電子郵件伺服器的封鎖輸入郵件，您需要判斷原因，並從 Spamhaus 網站移除區塊。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="b5c8f-107">若封鎖來源 IP 位址屬於其他人的輸入郵件，位址擁有者必須從 Spamhaus 網站中移除該塊。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="b5c8f-108">如果 IP 位址位於原則封鎖清單中 (PBL) ，擁有者可以指派不同的靜態 IP 位址，或移除 PBL 中的位址。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="b5c8f-109">若封鎖從您的網域連線到 Microsoft 的輸出郵件，如果郵件是透過協力廠商服務路由傳送，您就會收到此錯誤。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="b5c8f-110">您可以使用 WHOIS 查閱工具來找出封鎖的 IP 位址擁有者。</span><span class="sxs-lookup"><span data-stu-id="b5c8f-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
