---
title: 使用 Exchange Online PowerShell 啟用特定網域的 DKIM
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
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736032"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>使用 Exchange Online PowerShell 啟用特定網域的 DKIM

如果您無法在系統管理中心建立 DKIM DNS 記錄，請嘗試使用 Exchange Online PowerShell。 

若要使用 Exchange Online PowerShell 建立 DKIM DNS 記錄，請執行下列步驟：

1. 以系統管理員身分開啟 Windows PowerShell，並在所述的順序中執行下列命令：

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
如果您無法連線至 Exchange Online PowerShell，請參閱 [Connect To Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)。

2. 當您連線至 Exchange Online PowerShell 後，請執行下列命令：

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 在成功執行上述命令之後，請執行下列命令終止 Exchange Online PowerShell 會話：

    `Remove-PSSession $Session` 



