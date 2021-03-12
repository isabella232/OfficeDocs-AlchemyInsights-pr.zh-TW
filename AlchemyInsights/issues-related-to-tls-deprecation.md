---
title: 由於 TLS 1.0 和 TLS 1.1 停用，無法將電子郵件傳送至/從 Office 365 傳送/接收
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50726910"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>由於 TLS 1.0 和 TLS 1.1 停用，無法將電子郵件傳送至/從 Office 365 傳送/接收

如郵件中心後 MC229914 所確認，TLS 1.0 和 TLS 1.1 已過時，已開始強制執行 Exchange Online 郵件流程端點。 Office 365 不久將不再接受 TLS 1.0 和 TLS 1.1 來自外部來源的電子郵件連線。 此外，Exchange Online 永遠不會使用 TLS 1.0 或1.1 傳送輸出電子郵件。 如果您因 TLS 1.0 或1.1 停用而面臨問題，您可能會遇到下列其中一個錯誤-

- 寄件者正在進行 NDR 回復-' 421 4.4.2 Connection 由於 SocketError ' 已中斷」
- 傳送電子郵件給官365的 On-Premises 伺服器佇列檢視器錯誤-' 421 4.4.2 Connection 因 SocketError 而中斷
- 傳送電子郵件到 Office 365 之伺服器上的傳送連接器 [通訊協定記錄](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 檔發生錯誤-TLS 協商失敗，錯誤 SocketError
- 在傳送或接收連接器通訊協定記錄中發生錯誤-' 451 5.7.3 必須簽發 STARTTLS 命令 first '

如果您遇到上述任何錯誤，請檢查下列登錄機碼，確定傳送或接收電子郵件的伺服器是否已啟用 TLS 1.2。

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2][HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ 用戶端] **"DisabledByDefault" = dword： 00000000 "Enabled" = dword： 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ 伺服器] **"DisabledByDefault" = dword： 00000000 "Enabled" = dword： 00000001**

若您在上述登錄機碼中進行任何變更，以啟用 TLS 1.2，請重新開機伺服器，讓變更生效。 此外，請確定您已安裝最新的 Windows 和 Exchange 更新。

如需詳細資訊，請參閱：

- [Exchange Server TLS 指導方針，第1部分：準備好進行 TLS 1.2-Microsoft 技術社區](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS 指南第2部分：啟用 TLS 1.2 並識別不是使用它的用戶端-Microsoft 技術社區](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [若 TLS 版本無法與 Exchange Online （Microsoft 技術群組）商定，請瞭解電子郵件案例](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
