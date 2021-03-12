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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="05229-102">由於 TLS 1.0 和 TLS 1.1 停用，無法將電子郵件傳送至/從 Office 365 傳送/接收</span><span class="sxs-lookup"><span data-stu-id="05229-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="05229-103">如郵件中心後 MC229914 所確認，TLS 1.0 和 TLS 1.1 已過時，已開始強制執行 Exchange Online 郵件流程端點。</span><span class="sxs-lookup"><span data-stu-id="05229-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="05229-104">Office 365 不久將不再接受 TLS 1.0 和 TLS 1.1 來自外部來源的電子郵件連線。</span><span class="sxs-lookup"><span data-stu-id="05229-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="05229-105">此外，Exchange Online 永遠不會使用 TLS 1.0 或1.1 傳送輸出電子郵件。</span><span class="sxs-lookup"><span data-stu-id="05229-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="05229-106">如果您因 TLS 1.0 或1.1 停用而面臨問題，您可能會遇到下列其中一個錯誤-</span><span class="sxs-lookup"><span data-stu-id="05229-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="05229-107">寄件者正在進行 NDR 回復-' 421 4.4.2 Connection 由於 SocketError ' 已中斷」</span><span class="sxs-lookup"><span data-stu-id="05229-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="05229-108">傳送電子郵件給官365的 On-Premises 伺服器佇列檢視器錯誤-' 421 4.4.2 Connection 因 SocketError 而中斷</span><span class="sxs-lookup"><span data-stu-id="05229-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="05229-109">傳送電子郵件到 Office 365 之伺服器上的傳送連接器 [通訊協定記錄](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 檔發生錯誤-TLS 協商失敗，錯誤 SocketError</span><span class="sxs-lookup"><span data-stu-id="05229-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="05229-110">在傳送或接收連接器通訊協定記錄中發生錯誤-' 451 5.7.3 必須簽發 STARTTLS 命令 first '</span><span class="sxs-lookup"><span data-stu-id="05229-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="05229-111">如果您遇到上述任何錯誤，請檢查下列登錄機碼，確定傳送或接收電子郵件的伺服器是否已啟用 TLS 1.2。</span><span class="sxs-lookup"><span data-stu-id="05229-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="05229-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2][HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ 用戶端] **"DisabledByDefault" = dword： 00000000 "Enabled" = dword： 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ 伺服器] **"DisabledByDefault" = dword： 00000000 "Enabled" = dword： 00000001**</span><span class="sxs-lookup"><span data-stu-id="05229-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="05229-113">若您在上述登錄機碼中進行任何變更，以啟用 TLS 1.2，請重新開機伺服器，讓變更生效。</span><span class="sxs-lookup"><span data-stu-id="05229-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="05229-114">此外，請確定您已安裝最新的 Windows 和 Exchange 更新。</span><span class="sxs-lookup"><span data-stu-id="05229-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="05229-115">如需詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="05229-115">For more information, see:</span></span>

- [<span data-ttu-id="05229-116">Exchange Server TLS 指導方針，第1部分：準備好進行 TLS 1.2-Microsoft 技術社區</span><span class="sxs-lookup"><span data-stu-id="05229-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="05229-117">Exchange Server TLS 指南第2部分：啟用 TLS 1.2 並識別不是使用它的用戶端-Microsoft 技術社區</span><span class="sxs-lookup"><span data-stu-id="05229-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="05229-118">若 TLS 版本無法與 Exchange Online （Microsoft 技術群組）商定，請瞭解電子郵件案例</span><span class="sxs-lookup"><span data-stu-id="05229-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
