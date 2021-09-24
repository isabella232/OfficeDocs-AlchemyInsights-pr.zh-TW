---
title: 從 Microsoft 名稱伺服器改回管理您自己的 DNS 記錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2021
ms.locfileid: "59481847"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>從 Microsoft 名稱伺服器改回管理您自己的 DNS 記錄

您先前將 NS 記錄變更為指向 Microsoft (ns1.bdm.microsoftonline.com)，但現在决定管理您自己的 DNS 記錄：

在您的網域註冊機構網站上，將名稱伺服器改回為您的註冊機構或上一設定。 若不熟悉 DNS，請連絡網域註冊機構支援人員。 請注意名稱伺服器變更最多可能需要 48 小時才會傳播。 

1. 在 Microsoft 365 系統管理入口網站中，前往 **[設定]** > [**[網域]**](https://admin.microsoft.com/Adminportal/Home#/Domains)，選取網域旁的核取方塊，然後選取 **[管理 DNS]**。 

2. 在精靈中，選取 **[新增您自己的 DNS 記錄]**，然後完成精靈。 這將變更您的 DNS 的管理方式，然後讓您新增支援選取之服務所需的自訂 DNS 記錄。

或者，若您將名稱伺服器記錄變更為 Microsoft 並擁有網站，則可以為該網站新增 DNS 記錄，而非改回名稱伺服器。 如需詳細資訊，請參閱 [更新 DNS 記錄以便向目前的主機服務提供者保留網站](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)。


