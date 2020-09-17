---
title: Project Online 處於唯讀狀態
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: ad2a9f95bf30708772edb166945f3f42e0f1f503
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801643"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="78717-102">Project Online 處於唯讀狀態</span><span class="sxs-lookup"><span data-stu-id="78717-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="78717-103">Project Online 可能會達到唯讀狀態的常見原因有三個：</span><span class="sxs-lookup"><span data-stu-id="78717-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="78717-104">組織僅有 Project Online 基本版授權 (s) 。</span><span class="sxs-lookup"><span data-stu-id="78717-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="78717-105">這不足以讓網站保持在活狀態，最終會進行取消布建。</span><span class="sxs-lookup"><span data-stu-id="78717-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="78717-106">我們會將網站設為唯讀狀態，讓系統管理員知道問題是否正確，而且可以取得正確的授權。</span><span class="sxs-lookup"><span data-stu-id="78717-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="78717-107">系統管理員必須新增 Project Online 專業版和/或特優授權。</span><span class="sxs-lookup"><span data-stu-id="78717-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="78717-108">該網站會在該點上以唯讀狀態退出。</span><span class="sxs-lookup"><span data-stu-id="78717-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="78717-109">如需詳細資訊，請參閱 [比較專案管理解決方案](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)。</span><span class="sxs-lookup"><span data-stu-id="78717-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="78717-110">已達到指定的配額。</span><span class="sxs-lookup"><span data-stu-id="78717-110">Assigned quota has been reached.</span></span> <span data-ttu-id="78717-111">如需詳細資訊，請參閱 [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)。</span><span class="sxs-lookup"><span data-stu-id="78717-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="78717-112">請檢查 [Project Online 中的時段報告資料匯總](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) ，以查看報告細微性可能會對配額使用量產生什麼影響。</span><span class="sxs-lookup"><span data-stu-id="78717-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="78717-113">唯讀可能是在維護期間可能發生的暫時性情況。</span><span class="sxs-lookup"><span data-stu-id="78717-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="78717-114">我們的客戶甚至不會注意到大部分的維護，您也不會看到這種情況，但有時會有一些很短的唯讀時段。</span><span class="sxs-lookup"><span data-stu-id="78717-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
