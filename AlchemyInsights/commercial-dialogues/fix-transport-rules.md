---
title: 修正傳輸規則
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50736153"
---
# <a name="fix-transport-rules"></a><span data-ttu-id="a67d6-102">修正傳輸規則</span><span class="sxs-lookup"><span data-stu-id="a67d6-102">Fix transport rules</span></span>

<span data-ttu-id="a67d6-103">自訂郵件流程規則會影響此郵件。</span><span class="sxs-lookup"><span data-stu-id="a67d6-103">A custom mail flow rule affected this message.</span></span> <span data-ttu-id="a67d6-104">若要查看確切的規則，請執行下列動作：</span><span class="sxs-lookup"><span data-stu-id="a67d6-104">To review the exact rule, do the following:</span></span>

1. <span data-ttu-id="a67d6-105">在提交結果的 [ **其他資訊**] 下，記下 **GUID** 或 **原則名稱**。</span><span class="sxs-lookup"><span data-stu-id="a67d6-105">In the submission results, under **Additional information**, note the **GUID** or the **Policy Name**.</span></span>
2. <span data-ttu-id="a67d6-106">啟動 Exchange 管理命令介面。</span><span class="sxs-lookup"><span data-stu-id="a67d6-106">Launch Exchange Management Shell.</span></span> <span data-ttu-id="a67d6-107">如需詳細資訊，請參閱 [開啟 Exchange 管理命令](https://go.microsoft.com/fwlink/?linkid=2101432)介面。</span><span class="sxs-lookup"><span data-stu-id="a67d6-107">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
3. <span data-ttu-id="a67d6-108">使用提交) 中的 GUID 執行此命令 (：  **Get-TransportRule 身分 "GUID" | fl \* 描述**\*</span><span class="sxs-lookup"><span data-stu-id="a67d6-108">Run this command (using the GUID from your submission):  **Get-TransportRule -identity "GUID" | fl \* Description**\*</span></span>
4. <span data-ttu-id="a67d6-109">請複查描述，以查看影響郵件的設定條件。</span><span class="sxs-lookup"><span data-stu-id="a67d6-109">Review the description to see the configured conditions that affected the message.</span></span>

<span data-ttu-id="a67d6-110">若要深入瞭解，請參閱 [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)。</span><span class="sxs-lookup"><span data-stu-id="a67d6-110">To learn more, see [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).</span></span>
