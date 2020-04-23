---
title: 修正 DKIM 安裝問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717553"
---
# <a name="fix-dkim-setup-issues"></a>修正 DKIM 安裝問題

如果您在為自訂網域啟用 DKIM 時遇到問題，請使用下列步驟：

- 大部分 DKIM 的設定問題都與不正確的 DNS 記錄有關。 確認 DKIM CNAME 記錄（**不**是 TXT 記錄）的格式設定正確。 如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365)。

- 在您的網域（通常是您的網域註冊機構）的 DNS 主機服務上建立或更新 DKIM DNS 記錄之後，請等候 DNS 記錄傳播。

- 如果您無法在系統管理中心建立 DKIM DNS 記錄，您可以\<將 CustomDomain\>取代為您的自訂網域（例如，contoso.com），然後在[Exchange Online](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行此命令`New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`PowerShell：。
