---
title: 以 Microsoft 365 群組傳送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: 51bd8a10c3da23941cc16d7ba860406f8477044a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740142"
---
# <a name="send-as-microsoft-365-group"></a>以 Microsoft 365 群組傳送

您可以指派 [傳送為] 權限，以允許特定使用者以 Microsoft 365 群組的方式傳送郵件：  

1. 連線至 Exchange Online PowerShell。  

2. 執行下列命令：  

    Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs

如需詳細資料，請參閱[允許成員使用「傳送為」或「代理傳送者」功能](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide)。