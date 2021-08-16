---
title: 使用 Exchange Online PowerShell 來啟用特定網域的 DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070282"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>使用 Exchange Online PowerShell 來啟用特定網域的 DKIM

如果您無法在系統管理中心建立 DKIM DNS 記錄，請嘗試使用 Exchange Online PowerShell。 

若要使用 Exchange Online PowerShell 建立 DKIM DNS 記錄，請執行下列步驟：

1. 以系統管理員身分開啟 Windows PowerShell，並在所述的順序中執行下列命令：

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
如果您在連線至 Exchange Online PowerShell 時發生問題，請參閱[連線 to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)。

2. 當您連線至 Exchange Online PowerShell 之後，請執行下列命令：

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 在成功執行上述命令之後，請執行下列命令終止 Exchange Online PowerShell 會話：

    `Remove-PSSession $Session` 



