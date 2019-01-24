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
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460898"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>取代了 EOP 輸出 IP 位址範圍

我們已偵測到 （如果未由 2018 年 10 月 26、 修正） 可能會自動換行郵件流程給您的內部或外部目的地貴組織的潛在問題。為先前溝通簡化 IP 位址範圍管理，我們正在合併可用來傳送和接收 Office 365 外部的電子郵件的 Exchange Online Protection (EOP) IP 位址範圍。我們分析表示一或多個外部電子郵件來源或您已設定郵件流程連接器中的目的地不接受來自 IP 位址範圍顯示[以下](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的連線。
  
處理之前年 10 月 26 以確保這些來源和目的地會接受連線到與所有[發佈 EOP IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。
  
如需這項變更的詳細資訊，請參閱訊息中心張貼訊息[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。
  
 **請注意**： 如果之前使用 HTML、 XML 及 RSS 透過 IP 或 URL 發佈端點更新，您也應該移轉至新的 web 服務的自動化這些類型的更新。如需詳細資訊，請參閱[Office 365 端點類別與 Office 365 IP 位址及 URL web 服務](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
  

