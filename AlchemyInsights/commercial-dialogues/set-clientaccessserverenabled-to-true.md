---
title: 將 ClientAccessServerEnabled 設定為 True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994856"
---
# <a name="set-clientaccessserverenabled-to-true"></a>將 ClientAccessServerEnabled 設定為 True

如果您無法開啟加密的電子郵件，而是查看 **rpmsg** 附件，請執行下列步驟：

1. 連線至 Exchange Online PowerShell。

> [!NOTE]
> 若要連線至 Exchange Online PowerShell，您必須使用全域系統管理員或 Exchange 的系統管理員帳戶登入。

   a. 開啟 Windows PowerShell，然後執行下列命令：`$UserCredential = Get-Credential`
b. 在 [ **Windows PowerShell 認證要求**] 對話方塊中，輸入您的公司或學校帳戶，以及密碼 c。 按一下 ****[確定]。 

2. 執行下列命令以建立新的會話：

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. 執行下列命令：
    
    `Import-PSSession $Session -DisableNameChecking`

3. 執行 `Get-IRMConfiguration` 命令。

4. 檢查 **ClientAccessServerEnabled** 設定。 

    a. 如果 **ClientAccessServerEnabled** 設定設為 **False**，請執行下列 Cmdlet： `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> 請務必使用下列命令來關閉 powershell 會話： `Remove-PSSession $Session`

如需詳細資訊，請參閱[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)。

