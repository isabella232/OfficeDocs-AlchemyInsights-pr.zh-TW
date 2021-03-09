---
title: 建立共用信箱時的 Proxy 位址錯誤
ms.author: pebaum
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ece4bcce-1053-4ed3-a194-9d0af8f73c6f
ms.custom:
- "19"
- "6"
ms.openlocfilehash: ab491e883ab294f08d0b5d2e686dc059b468d29f
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/09/2021
ms.locfileid: "50568281"
---
# <a name="proxy-address-error-while-creating-a-mailbox-or-other-email-enabled-object"></a>建立信箱或其他具有電子郵件功能的物件時出現 Proxy 位址錯誤

如果您嘗試建立具有電子郵件功能的物件 (信箱、共用信箱等 ) 並收到錯誤「proxy 位址 "SMTP:alias@domain.com" 已使用。 ... "，您所選擇的電子郵件地址已經由您組織中的另一個具有電子郵件功能的物件所使用。
  
您需要找出具有此電子郵件地址的使用者、群組、共用信箱或公用資料夾，並將其刪除或變更其電子郵件地址。 然後，您就可以使用已釋放的電子郵件地址來建立新的具有電子郵件功能的物件。 在首頁上使用搜尋來尋找。 您也可以使用下列 Exchange Online PowerShell 命令來搜尋該專案：

`
    Get-EXORecipient -Filter "EmailAddresses -eq 'email@contoso.onmicrosoft.com'"
`
  
如果您不想刪除現有的電子郵件地址，請為您要建立的新物件選擇新的電子郵件地址。
  