---
title: 將Wix網站與Microsoft Office 365購買或託管域一起使用
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001516"
- "3582"
ms.openlocfilehash: 522392d41aa8f84f1f4684ccdbd37d68636be07e
ms.sourcegitcommit: cbed17334557c1dfa471623f8d5e735f72e697da
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/28/2020
ms.locfileid: "47300688"
---
# <a name="using-wix-website-with-office-365-purchased-or-managed-domains"></a>將Wix網站與Microsoft Office 365購買或託管域一起使用

- [更新 DNS 記錄以便向目前的主機服務提供者保留網站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)
- Wix文章 [ 使用指向方法將網域連接到Wix] 建議使用指向（透過以上連結新增DNS記錄），而非在使用Microsoft Office 365時更改服務器名稱
- 如果您仍然選擇將名稱伺服器變更為 Wix，您將  [需要在Wix for Microsoft 創建 DNS 記錄](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix?view=o365-worldwide)
- 如果您的網域是向 Microsoft 購買，則不能變更伺服器名稱。 如果您必須變更伺服器名稱，在60天之後，您必須將 Microsoft 購買的網域  [轉移到另一個託管主機服務提供者](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)