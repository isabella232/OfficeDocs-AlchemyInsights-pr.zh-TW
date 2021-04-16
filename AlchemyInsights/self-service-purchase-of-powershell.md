---
title: PowerShell 的自助購買
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797712"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="e06ec-102">PowerShell 的自助購買</span><span class="sxs-lookup"><span data-stu-id="e06ec-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="e06ec-103">若要使用 MSCommerce PowerShell 模組，您必須將其安裝在具有 TLS 1.2 (本機系統管理員許可權) 的 Windows 10 裝置上。</span><span class="sxs-lookup"><span data-stu-id="e06ec-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="e06ec-104">匯入並連接至 MSCommerce 模組。</span><span class="sxs-lookup"><span data-stu-id="e06ec-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="e06ec-105">當系統提示登入時，您必須使用通用或計費系統管理員角色認證。</span><span class="sxs-lookup"><span data-stu-id="e06ec-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="e06ec-106">如果您沒有 TLS 1.2，當您嘗試取得或更新原則時，可能會收到下列錯誤：</span><span class="sxs-lookup"><span data-stu-id="e06ec-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="e06ec-107">*ErrorMessage-基礎 connection 已關閉：傳送時發生意外的錯誤*。</span><span class="sxs-lookup"><span data-stu-id="e06ec-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



