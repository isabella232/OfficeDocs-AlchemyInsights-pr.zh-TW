---
title: 1065 取代的 EOP 輸出 IP 位址 rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2019
ms.locfileid: "28278669"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="30edd-102">取代了 EOP 輸出 IP 位址範圍</span><span class="sxs-lookup"><span data-stu-id="30edd-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="30edd-p101">我們已偵測到 （如果未由 2018 年 10 月 26、 修正） 可能會自動換行郵件流程給您的內部或外部目的地貴組織的潛在問題。為先前溝通簡化 IP 位址範圍管理，我們正在合併可用來傳送和接收 Office 365 外部的電子郵件的 Exchange Online Protection (EOP) IP 位址範圍。我們分析表示一或多個外部電子郵件來源或您已設定郵件流程連接器中的目的地不接受來自 IP 位址範圍顯示[以下](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的連線。</span><span class="sxs-lookup"><span data-stu-id="30edd-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="30edd-106">處理之前年 10 月 26 以確保這些來源和目的地會接受連線到與所有[發佈 EOP IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。</span><span class="sxs-lookup"><span data-stu-id="30edd-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="30edd-107">如需這項變更的詳細資訊，請參閱訊息中心張貼訊息[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。</span><span class="sxs-lookup"><span data-stu-id="30edd-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="30edd-p102">**請注意**： 如果之前使用 HTML、 XML 及 RSS 透過 IP 或 URL 發佈端點更新，您也應該移轉至新的 web 服務的自動化這些類型的更新。如需詳細資訊，請參閱[Office 365 端點類別與 Office 365 IP 位址及 URL web 服務](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。</span><span class="sxs-lookup"><span data-stu-id="30edd-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

