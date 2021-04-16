---
title: 啟用內嵌舊版對話方塊以開啟報告
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814255"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="672ae-102">啟用內嵌舊版對話方塊以開啟報告</span><span class="sxs-lookup"><span data-stu-id="672ae-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="672ae-103">**徵狀**</span><span class="sxs-lookup"><span data-stu-id="672ae-103">**Symptom**</span></span>

<span data-ttu-id="672ae-104">使用者無法開啟報告。</span><span class="sxs-lookup"><span data-stu-id="672ae-104">Users are unable to open reports.</span></span> <span data-ttu-id="672ae-105">「發生錯誤。</span><span class="sxs-lookup"><span data-stu-id="672ae-105">"Something has gone wrong.</span></span> <span data-ttu-id="672ae-106">如需詳細資訊，請查看技術詳細資料。」</span><span class="sxs-lookup"><span data-stu-id="672ae-106">Check technical details for more details."</span></span>

<span data-ttu-id="672ae-107">**原因**</span><span class="sxs-lookup"><span data-stu-id="672ae-107">**Cause**</span></span>

<span data-ttu-id="672ae-108">在 UCI 中無法載入報告，出現錯誤：「表單描述項為 Null 或未定義」。</span><span class="sxs-lookup"><span data-stu-id="672ae-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="672ae-109">UCI 中的報告仍然需要舊版對話方塊，因此客戶的系統必須啟用 *allowlegacydialogsembedding*。</span><span class="sxs-lookup"><span data-stu-id="672ae-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="672ae-110">**解決方案**</span><span class="sxs-lookup"><span data-stu-id="672ae-110">**Solution**</span></span>

1. <span data-ttu-id="672ae-111">移至 **[設定] > [管理] > [系統設定] > [一般] 索引標籤**。</span><span class="sxs-lookup"><span data-stu-id="672ae-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="672ae-112">將「在整合介面瀏覽器用戶端中，啟用某些舊版對話方塊的嵌入」設定為 **是**。</span><span class="sxs-lookup"><span data-stu-id="672ae-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
