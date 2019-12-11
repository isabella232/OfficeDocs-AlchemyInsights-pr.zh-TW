---
title: 無法存取公用資料夾
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959486"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook 無法連線至公用資料夾

如果公用資料夾存取無法正常的幾個使用者，請嘗試下列方法：

連接至 EXO PowerShell，並設定 DefaultPublicFolderMailbox 問題的使用者帳戶，以符合一個工作的使用者帳戶。

範例：

Get-mailbox WorkingUser |ft DefaultPublicFolderMailbox EffectivePublicFolderMailbox

Set-mailbox ProblemUser DefaultPublicFolderMailbox\<值從上一個命令>

請等候至少一小時，變更才會生效。