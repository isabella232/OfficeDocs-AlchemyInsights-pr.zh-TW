---
title: 自助服務購買的 PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091669"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="9e709-102">自助服務購買的 PowerShell</span><span class="sxs-lookup"><span data-stu-id="9e709-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="9e709-103">若要使用 MSCommerce PowerShell 模組，您必須安裝在 Windows 10 裝置與 TLS 1.2 版 （需要本機系統管理員權限）。</span><span class="sxs-lookup"><span data-stu-id="9e709-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="9e709-104">匯入並連線至 MSCommerce 模組。</span><span class="sxs-lookup"><span data-stu-id="9e709-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="9e709-105">出現提示時登入，您必須使用全域或計費系統管理員角色的認證。</span><span class="sxs-lookup"><span data-stu-id="9e709-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="9e709-106">如果您不需要 TLS 1.2，您可能會嘗試取得或更新原則時收到下列錯誤：</span><span class="sxs-lookup"><span data-stu-id="9e709-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="9e709-107">*ErrorMessage-基礎連接已關閉： 傳送發生意外的錯誤*。</span><span class="sxs-lookup"><span data-stu-id="9e709-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



