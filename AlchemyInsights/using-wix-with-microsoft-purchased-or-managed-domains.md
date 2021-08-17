---
title: 使用 Wix 網站搭配向 Microsoft 購買或受管理的網域
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5855"
- "9003096"
ms.openlocfilehash: dd0f8beb8f1871c2c43ac14a7f6d1cce79386fcc353bb2a690ba184904ca5857
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083725"
---
# <a name="using-a-wix-website-with-microsoft-purchased-or-managed-domains"></a>使用 Wix 網站搭配向 Microsoft 購買或受管理的網域

如需如何使用 Wix 網站搭配向 Microsoft 購買或受管理的網域的相關資訊，請參閱[更新 DNS 記錄以便向目前的代管提供者保留網站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)。

如需詳細資訊，請參閱： 

- Wix 文章「使用指向方法將網域連接至 Wix」(英文) 建議新增 DNS 記錄 (如以上連結中所概述)，而非在使用 Microsoft 365 時變更名稱伺服器。

- 如果您選擇將名稱伺服器變更為 Wix，則必須在 Wix 為 Microsoft 建立 DNS 記錄。 如需詳細資訊，請參閱[在 Wix 為 Microsoft 建立 DNS 記錄](https://docs.microsoft.com/microsoft-365/admin/dns/create-dns-records-at-wix)。

- 如果您的網域是向 Microsoft 購買，則不能變更名稱伺服器。 如果您必須變更名稱伺服器，必須在 60天之後，將向 Microsoft 購買的網域轉移到另一個代管提供者。 如需詳細資訊，請參閱 [將網域從 Microsoft 傳送到另一個主機](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)。
