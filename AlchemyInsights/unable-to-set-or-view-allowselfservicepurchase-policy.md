---
title: 無法設定或查看 AllowSelfServicePurchase 原則
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826082"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="de0e1-102">無法設定或查看 AllowSelfServicePurchase 原則</span><span class="sxs-lookup"><span data-stu-id="de0e1-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="de0e1-103">當您嘗試設定或查看 AllowSelfServicePurchase 原則時，會收到下列錯誤訊息：</span><span class="sxs-lookup"><span data-stu-id="de0e1-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="de0e1-104">*HandleError：無法使用 PolicyId ' AllowSelfServicePurchase ' 取得產品原則，ErrorMessage-基礎 connection 已關閉：傳送時發生意外的錯誤。*</span><span class="sxs-lookup"><span data-stu-id="de0e1-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="de0e1-105">這可能是因為舊版本的傳輸層安全性 (TLS) 。</span><span class="sxs-lookup"><span data-stu-id="de0e1-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="de0e1-106">若要連接 MSCommerce 服務，您必須使用 TLS 1.2 或更新版本。</span><span class="sxs-lookup"><span data-stu-id="de0e1-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="de0e1-107">請嘗試下列步驟，將 TLS 通訊協定啟用/設定為1.2、驗證及重試。</span><span class="sxs-lookup"><span data-stu-id="de0e1-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="de0e1-108">在 PowerShell 命令提示字元處 (PS C： \) 輸入下列命令，將 TLS 通訊協定設定為版本1.2：</span><span class="sxs-lookup"><span data-stu-id="de0e1-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="de0e1-109">使用下列命令，確認 TLS 通訊協定 (s) 在使用中：</span><span class="sxs-lookup"><span data-stu-id="de0e1-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="de0e1-110">視需要重試 Get 或 Update 命令。</span><span class="sxs-lookup"><span data-stu-id="de0e1-110">Retry the Get or Update commands as needed.</span></span>

