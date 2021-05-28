---
title: 診斷以啟用 Exchange Online 通訊協定的基本驗證
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11392"
- "9006699"
ms.openlocfilehash: 8952aba3dc6b5abcf56776d81eddd9b50db33c7f
ms.sourcegitcommit: d3a739b75d521837660ce151190a7e232e4eeadb
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/27/2021
ms.locfileid: "52689935"
---
# <a name="diagnostic-to-enable-basic-authentication-for-exchange-online-protocols"></a><span data-ttu-id="09b68-102">診斷以啟用 Exchange Online 通訊協定的基本驗證</span><span class="sxs-lookup"><span data-stu-id="09b68-102">Diagnostic to enable Basic authentication for Exchange Online protocols</span></span>

<span data-ttu-id="09b68-103">透過使用此診斷，您可以為 Exchange Online 通訊協定 (例如 POP3、IMAP4、Exchange ActiveSync、Exchange Web 服務、離線通訊錄、MAPI、RPC 和遠端 PowerShell) 啟用基本驗證，Microsoft 最近可能已為貴組織停用此驗證。</span><span class="sxs-lookup"><span data-stu-id="09b68-103">By using this diagnostic, you can enable Basic authentication for Exchange Online protocols such as POP3, IMAP4, Exchange ActiveSync, Exchange Web Services, Offline Address Book, MAPI, RPC and Remote PowerShell, which Microsoft might have disabled recently for your organization.</span></span> 

<span data-ttu-id="09b68-104">我們正在透過訊息中心傳送直接通訊，讓租用戶知道他們因為沒有任何使用量，因而已準備好關閉環境中的基本驗證，這可協助保護其環境免受相關安全性風險的影響。</span><span class="sxs-lookup"><span data-stu-id="09b68-104">We are sending direct communications through Message Center to let tenants know where they're ready to turn off Basic authentication in their environment due to no use, which will help protect their environments from related security risks.</span></span>