---
title: 以 Microsoft 365 群組傳送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/21/2020
ms.locfileid: "46852993"
---
# <a name="send-as-microsoft-365-group"></a>以 Microsoft 365 群組傳送

您可以指派 [傳送為] 權限，以允許特定使用者以 Microsoft 365 群組的方式傳送郵件：  

1. 連線至 Exchange Online PowerShell。  

2. 執行下列命令：  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

如需詳細資料，請參閱[允許成員使用「傳送為」或「代理傳送者」功能](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)。