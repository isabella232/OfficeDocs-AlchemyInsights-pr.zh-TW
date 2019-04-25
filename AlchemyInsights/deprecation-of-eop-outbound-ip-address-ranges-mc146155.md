---
title: 1065 deprecation > 的 EOP 輸出 IP 位址 rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 17beb1722142d94ea05b67ce5ed1f20f8b11375c
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32404812"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="b50a5-102">EOP 輸出 IP 位址範圍的 deprecation ></span><span class="sxs-lookup"><span data-stu-id="b50a5-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="b50a5-103">我們已偵測到與組織 （如果不進行修正所 2018 年 10 月 26 日） 可能會中斷郵件流程您的內部或外部目的地的潛在問題。</span><span class="sxs-lookup"><span data-stu-id="b50a5-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="b50a5-104">為先前溝通，以簡化 IP 位址範圍的管理，我們正在合併可用來傳送及接收 Office 365 外部的電子郵件的 Exchange Online Protection (EOP) IP 位址範圍。</span><span class="sxs-lookup"><span data-stu-id="b50a5-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="b50a5-105">我們的分析指出一或多個外部電子郵件來源] 或 [郵件流程連接器中已設定的目的地不接受來自 IP 位址範圍顯示[以下](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的連線。</span><span class="sxs-lookup"><span data-stu-id="b50a5-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="b50a5-106">處理之前年 10 月 26 以確保這些來源和目的地會接受連線到及傳送自所有[發佈 EOP IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。</span><span class="sxs-lookup"><span data-stu-id="b50a5-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="b50a5-107">如需這項變更的詳細資訊，請參閱訊息中心文章[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。</span><span class="sxs-lookup"><span data-stu-id="b50a5-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="b50a5-108">**附註**： 如果您先前使用透過 HTML、 XML、 和 RSS IP 或 URL 發佈端點更新，您也應該將移轉至新的 web 服務，用來自動執行這些類型的更新。</span><span class="sxs-lookup"><span data-stu-id="b50a5-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="b50a5-109">如需詳細資訊，請參閱[Office 365 端點類別和 Office 365 IP 位址和 URL web 服務](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。</span><span class="sxs-lookup"><span data-stu-id="b50a5-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
