---
title: 使用 Outlook 控制公用資料夾的存取權
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816731"
---
# <a name="control-access-to-public-folders-using-outlook"></a>使用 Outlook 控制公用資料夾的存取權

若要控制哪些使用者能夠使用 Outlook 存取公用資料夾：

1. 使用 `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true：允許使用者在 Outlook 中存取公用資料夾  
$false：避免使用者在 Outlook 中存取公用資料夾。 這是預設值。  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

附注：這個程式只能用來控制 Windows 的電腦版 Outlook 用戶端連線。 使用者可以使用 OWA 或 Mac 版 Outlook 繼續存取公用資料夾。

如需詳細資訊，請參閱 [Outlook 公用資料夾的受控制連線](https://aka.ms/controlpf) 以取得詳細資訊。
