---
title: 1554 Winsock 錯誤10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766160"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="0c388-102">Winsock 錯誤10061</span><span class="sxs-lookup"><span data-stu-id="0c388-102">Winsock error 10061</span></span>

<span data-ttu-id="0c388-103">此錯誤碼表示 Microsoft 無法與目標主機建立 TCP 通訊端（連接）。</span><span class="sxs-lookup"><span data-stu-id="0c388-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="0c388-104">這種錯誤最可能的原因是防火牆設定的問題。</span><span class="sxs-lookup"><span data-stu-id="0c388-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="0c388-105">若要修正此問題，請檢查這些設定：</span><span class="sxs-lookup"><span data-stu-id="0c388-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="0c388-106">使用[Microsoft 365 URLs 和 IP 位址範圍](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)中的資訊，確認您的防火牆設定</span><span class="sxs-lookup"><span data-stu-id="0c388-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="0c388-107">如果錯誤是 Exchange Online Protection （EOP）特有的，您就應該先前會收到[Exchange Online PROTECTION IP 位址](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)的變更通知。</span><span class="sxs-lookup"><span data-stu-id="0c388-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="0c388-108">確認網際網路服務提供者（ISP）未阻擋埠。</span><span class="sxs-lookup"><span data-stu-id="0c388-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="0c388-109">驗證連接器中的智慧主機和目標伺服器設定。</span><span class="sxs-lookup"><span data-stu-id="0c388-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="0c388-110">請注意，Microsoft 365 不會以這種方式封鎖*傳入*的連線。</span><span class="sxs-lookup"><span data-stu-id="0c388-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
