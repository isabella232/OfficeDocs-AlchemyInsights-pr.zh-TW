---
title: 1554 Winsock 錯誤 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 96a9cfd11941158ddf13655c74974e3eb800e570
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278527"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="37c67-102">Winsock 錯誤 10061</span><span class="sxs-lookup"><span data-stu-id="37c67-102">Winsock error 10061</span></span>

<span data-ttu-id="37c67-p101">此錯誤的程式碼表示 Office 365 無法建立與目標主機的 TCP 通訊端 （連線）。這項錯誤的很有可能原因為您的防火牆組態問題。若要修正此問題，檢查這些設定：</span><span class="sxs-lookup"><span data-stu-id="37c67-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="37c67-106">確認您的防火牆組態和[Office 365 Url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊</span><span class="sxs-lookup"><span data-stu-id="37c67-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="37c67-107">如果至 Exchange Online Protection (EOP) 特定錯誤，您應該已先前通知至[Exchange Online Protection IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更。</span><span class="sxs-lookup"><span data-stu-id="37c67-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="37c67-108">確認網際網路服務提供者 (ISP) 不會封鎖的連接埠。</span><span class="sxs-lookup"><span data-stu-id="37c67-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="37c67-109">確認您連接器在智慧主機和目標伺服器設定。</span><span class="sxs-lookup"><span data-stu-id="37c67-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="37c67-110">Office 365 不會封鎖以這種方式的*傳入*連線的附註。</span><span class="sxs-lookup"><span data-stu-id="37c67-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

