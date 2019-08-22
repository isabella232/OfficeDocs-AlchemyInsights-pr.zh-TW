---
title: 1554 Winsock 錯誤 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f54c7fc81c274871fbc22908ce0fb21500975d9e
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530775"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="7401c-102">Winsock 錯誤 10061</span><span class="sxs-lookup"><span data-stu-id="7401c-102">Winsock error 10061</span></span>

<span data-ttu-id="7401c-103">此錯誤代碼表示 Office 365 無法建立與目標主機的 TCP 通訊端 （連線）。</span><span class="sxs-lookup"><span data-stu-id="7401c-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="7401c-104">此錯誤最可能的原因是您的防火牆設定問題。</span><span class="sxs-lookup"><span data-stu-id="7401c-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="7401c-105">若要修正此問題，請檢查這些設定：</span><span class="sxs-lookup"><span data-stu-id="7401c-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="7401c-106">確認您的防火牆設定與[Office 365 Url 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊</span><span class="sxs-lookup"><span data-stu-id="7401c-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="7401c-107">如果此錯誤是特定至 Exchange Online Protection (EOP)，您應該已先前通知到[Exchange Online Protection IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更。</span><span class="sxs-lookup"><span data-stu-id="7401c-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="7401c-108">確認網際網路服務提供者 (ISP) 不會封鎖連接埠。</span><span class="sxs-lookup"><span data-stu-id="7401c-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="7401c-109">確認智慧主機 」 和 「 目標伺服器中的設定連接器。</span><span class="sxs-lookup"><span data-stu-id="7401c-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="7401c-110">請注意，Office 365 不會封鎖這種方式的*傳入*連線。</span><span class="sxs-lookup"><span data-stu-id="7401c-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
