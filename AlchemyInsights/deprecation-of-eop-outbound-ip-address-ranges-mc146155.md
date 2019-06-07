---
title: 1065 deprecation > 的 EOP 輸出 IP 位址 rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 9860845dea444847833d4c5cd01d49ea93473778
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752946"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a>EOP 輸出 IP 位址範圍的 deprecation >

我們已偵測到與組織 （如果不進行修正所 2018 年 10 月 26 日） 可能會中斷郵件流程您的內部或外部目的地的潛在問題。 為先前溝通，以簡化 IP 位址範圍的管理，我們正在合併可用來傳送及接收 Office 365 外部的電子郵件的 Exchange Online Protection (EOP) IP 位址範圍。 我們的分析指出一或多個外部電子郵件來源] 或 [郵件流程連接器中已設定的目的地不接受來自 IP 位址範圍顯示[以下](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的連線。

處理之前年 10 月 26 以確保這些來源和目的地會接受連線到及傳送自所有[發佈 EOP IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)。

如需這項變更的詳細資訊，請參閱訊息中心文章[MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)、 [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)或[MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274)。

**附註**： 如果您先前使用透過 HTML、 XML、 和 RSS IP 或 URL 發佈端點更新，您也應該將移轉至新的 web 服務，用來自動執行這些類型的更新。 如需詳細資訊，請參閱[Office 365 端點類別和 Office 365 IP 位址和 URL web 服務](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638)。
