---
title: 在 Linux 電腦上設定及驗證 MDATP 的排除專案
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/11/2021
ms.locfileid: "50735995"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="64dda-102">在 Linux 電腦上設定及驗證 MDATP 的排除專案</span><span class="sxs-lookup"><span data-stu-id="64dda-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="64dda-103">您可以從 MDATP 掃描中排除某些檔案、資料夾、程式及進程開啟的檔案。</span><span class="sxs-lookup"><span data-stu-id="64dda-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="64dda-104">排除項可協助避免對您的組織的軟體和檔案不正確或自訂的偵測。</span><span class="sxs-lookup"><span data-stu-id="64dda-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="64dda-105">排除也有助於降低 MDATP 所造成的效能問題。</span><span class="sxs-lookup"><span data-stu-id="64dda-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="64dda-106">若要深入瞭解，請參閱 [設定及驗證 MDATP For Linux 的排除](https://go.microsoft.com/fwlink/?linkid=2144517)專案。</span><span class="sxs-lookup"><span data-stu-id="64dda-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="64dda-107">本文所述的排除項不適用於其他 MDATP 的 Linux 功能，包括端點偵測和回應 (EDR) 。</span><span class="sxs-lookup"><span data-stu-id="64dda-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="64dda-108">使用本文所述方法排除的檔案，仍然可以觸發 EDR 警示和其他偵測功能。</span><span class="sxs-lookup"><span data-stu-id="64dda-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
