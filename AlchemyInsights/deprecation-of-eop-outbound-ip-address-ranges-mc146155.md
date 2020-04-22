---
title: 1065 EOP 輸出 IP 位址 rangesMC146155 的棄用
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704588"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="115c1-102">EOP 外寄 IP 位址範圍的否決</span><span class="sxs-lookup"><span data-stu-id="115c1-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="115c1-103">我們已偵測到貴組織的潛在問題（如果未在10月26日之前修正，2018）可能會將郵件流程破壞您的內部部署或外部目的地。</span><span class="sxs-lookup"><span data-stu-id="115c1-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="115c1-104">如前所述，為了簡化 IP 位址範圍管理，我們會合並 Exchange Online Protection （EOP） IP 位址範圍，以用於傳送和接收 Microsoft 365 以外的電子郵件。</span><span class="sxs-lookup"><span data-stu-id="115c1-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="115c1-105">我們的分析指出您在郵件流程連接器中設定的一或多個外部電子郵件來源或目的地，不會接受[此處](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)所顯示之 IP 位址範圍的連線。</span><span class="sxs-lookup"><span data-stu-id="115c1-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="115c1-106">在10月26之前行動，以確保這些來源和目的地會接受所有[發佈的 EOP IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的連線。</span><span class="sxs-lookup"><span data-stu-id="115c1-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="115c1-107">如需此變更的相關資訊，請參閱 Message Center post [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。</span><span class="sxs-lookup"><span data-stu-id="115c1-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="115c1-108">**附注**：如果您先前使用過透過 HTML、XML 和 RSS 進行端點更新的 IP 或 URL 發佈，您也應該遷移至新的 web 服務，以自動化這些類型的更新。</span><span class="sxs-lookup"><span data-stu-id="115c1-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="115c1-109">如需詳細資訊，請參閱[microsoft 365 端點類別和 microsoft 365 IP 位址和 URL web 服務](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。</span><span class="sxs-lookup"><span data-stu-id="115c1-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
