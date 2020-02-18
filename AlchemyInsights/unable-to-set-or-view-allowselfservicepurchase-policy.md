---
title: 無法設定或檢視 AllowSelfServicePurchase 原則
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091670"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="7204d-102">無法設定或檢視 AllowSelfServicePurchase 原則</span><span class="sxs-lookup"><span data-stu-id="7204d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="7204d-103">當嘗試設定或檢視 AllowSelfServicePurchase 原則，您會收到下列錯誤訊息：</span><span class="sxs-lookup"><span data-stu-id="7204d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="7204d-104">*HandleError： 無法擷取產品原則與 PolicyId 'AllowSelfServicePurchase' ErrorMessage-基礎連接已關閉： 傳送發生意外的錯誤。*</span><span class="sxs-lookup"><span data-stu-id="7204d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="7204d-105">這可能是由於較舊版本的傳輸層安全性 (TLS)。</span><span class="sxs-lookup"><span data-stu-id="7204d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="7204d-106">若要連接的 MSCommerce 服務，您需要使用 TLS 1.2 或更高版本。</span><span class="sxs-lookup"><span data-stu-id="7204d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="7204d-107">請嘗試下列步驟來啟用/集 1.2 TLS 通訊協定、 確認，然後重試。</span><span class="sxs-lookup"><span data-stu-id="7204d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="7204d-108">在 PowerShell 命令提示字元 (PS C:>\)輸入下列命令，以 TLS 通訊協定設 1.2 版：</span><span class="sxs-lookup"><span data-stu-id="7204d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="7204d-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="7204d-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="7204d-110">確認 TLS 通訊協定，在使用中，使用下列命令：</span><span class="sxs-lookup"><span data-stu-id="7204d-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="7204d-111">\[Net.ServicePointManager]::SecurityProtocol</span><span class="sxs-lookup"><span data-stu-id="7204d-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="7204d-112">視需要再試一次 [取得] 或 [更新命令。</span><span class="sxs-lookup"><span data-stu-id="7204d-112">Retry the Get or Update commands as needed.</span></span>

