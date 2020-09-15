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
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664233"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="fd18e-103">5.7.750 用戶端無法從未註冊的網域傳送郵件</span><span class="sxs-lookup"><span data-stu-id="fd18e-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="fd18e-104">當您租使用者中未布建的網域傳送大宗郵件時，就會發生此錯誤 (新增為公認的網域並驗證) 。</span><span class="sxs-lookup"><span data-stu-id="fd18e-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="fd18e-105">若要避免這種錯誤，您可以使用憑證型郵件流程連接器，其中憑證的網域為布建的網域，您也可以布建所有傳送網域。</span><span class="sxs-lookup"><span data-stu-id="fd18e-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
