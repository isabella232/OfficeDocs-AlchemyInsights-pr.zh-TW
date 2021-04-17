---
title: 將Wix網站與Microsoft Office 365購買或託管域一起使用
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: ef2e7278b1a70aedca1b2ad9c13c249bf8b09c00
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825938"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>將Wix網站與Microsoft Office 365購買或託管域一起使用

- [更新 DNS 記錄以便向目前的主機服務提供者保留網站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix文章 [ 使用指向方法將網域連接到Wix] 建議使用指向（透過以上連結新增DNS記錄），而非在使用Microsoft Office 365時更改服務器名稱
- 如果您仍然選擇將名稱伺服器變更為 Wix，您將  [需要在Wix for Microsoft 創建 DNS 記錄](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- 如果您的網域是向 Microsoft 購買，則不能變更伺服器名稱。 如果您必須變更伺服器名稱，在60天之後，您必須將 Microsoft 購買的網域  [轉移到另一個託管主機服務提供者](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)