---
title: 1048 5.7.750 服務無法使用。 已禁止用戶端從未註冊的網域傳送
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 5879c5996a28e8e9e61c696c51e7c590d1245ba1
ms.sourcegitcommit: edb9be61ff8c4df2a600f70952f6fa731c2093a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2021
ms.locfileid: "52774242"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="35223-103">5.7.750 用戶端無法從未註冊的網域傳送郵件</span><span class="sxs-lookup"><span data-stu-id="35223-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="35223-104">當您租使用者中未布建的網域傳送大宗郵件時，就會發生此錯誤 (新增為公認的網域並驗證) 。</span><span class="sxs-lookup"><span data-stu-id="35223-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="35223-105">若要避免這種錯誤，您可以使用憑證型郵件流程連接器，其中憑證的網域為布建的網域，您也可以布建所有傳送網域。</span><span class="sxs-lookup"><span data-stu-id="35223-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>

<span data-ttu-id="35223-106">如需詳細資訊，請參閱[修正 Exchange Online 中錯誤碼為 5.7.700 到 5.7.750 的電子郵件傳遞問題](https://go.microsoft.com/fwlink/?linkid=2164955)。</span><span class="sxs-lookup"><span data-stu-id="35223-106">For more information, see [Fix email delivery issues for error codes 5.7.700 through 5.7.750 in Exchange Online](https://go.microsoft.com/fwlink/?linkid=2164955).</span></span>