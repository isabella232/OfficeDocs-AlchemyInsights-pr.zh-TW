---
title: 設定測試人員風險管理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002284"
- "4405"
ms.openlocfilehash: 3cde8bb419d79506e101cd75fde6fcb69aa2441c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800959"
---
# <a name="set-up-insider-risk-management"></a><span data-ttu-id="8fbdb-102">設定測試人員風險管理</span><span class="sxs-lookup"><span data-stu-id="8fbdb-102">Set up insider risk management</span></span>

<span data-ttu-id="8fbdb-103">使用測試人員風險管理原則來識別危險的活動和管理工具，以針對組織中的風險警示採取動作。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-103">Use insider risk management policies to identify risky activities and management tools to take action on risk alerts in your organization.</span></span> <span data-ttu-id="8fbdb-104">開始使用測試人員風險管理之前，您應先確認 **Microsoft 365 訂閱**。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-104">Before you get started with insider risk management, you should confirm your **Microsoft 365 subscription**.</span></span> <span data-ttu-id="8fbdb-105">若要存取並使用測試人員風險管理，貴組織**必須**具備下列其中一種訂閱：</span><span class="sxs-lookup"><span data-stu-id="8fbdb-105">To access and use insider risk management, your organization **must** have one of the following subscriptions:</span></span>

- <span data-ttu-id="8fbdb-106">**Microsoft 365 E5** 訂閱。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-106">**Microsoft 365 E5** subscription.</span></span>

- <span data-ttu-id="8fbdb-107">含 Microsoft E5 合規性附加元件的 **Microsoft 365 E3** 訂閱。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-107">**Microsoft 365 E3** subscription with the Microsoft E5 compliance add-on.</span></span>

<span data-ttu-id="8fbdb-108">如果您沒有 **Microsoft 365 E5** 方案，且想要試用測試人員風險管理，您可以將 Microsoft 365 新增至現有的訂閱，或註冊 Microsoft 365 企業版 E5 的試用版。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-108">If you don't have an existing **Microsoft 365 E5** plan and want to try insider risk management, you can add Microsoft 365 to your existing subscription or Sign up for a trial of Microsoft 365 Enterprise E5.</span></span>

<span data-ttu-id="8fbdb-109">使用測試人員風險管理的基本步驟包括：</span><span class="sxs-lookup"><span data-stu-id="8fbdb-109">The basic steps for using Insider Risk Management include:</span></span>

1. <span data-ttu-id="8fbdb-110">為測試人員風險管理啟用權限。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-110">Enable permissions for insider risk management.</span></span>

2. <span data-ttu-id="8fbdb-111">啟用稽核記錄。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-111">Enable the audit log.</span></span>

3. <span data-ttu-id="8fbdb-112">設定範本的必要條件 (選用)。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-112">Configure prerequisites for template (optional).</span></span>

4. <span data-ttu-id="8fbdb-113">設定測試人員風險設定。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-113">Configure insider risk settings.</span></span>

5. <span data-ttu-id="8fbdb-114">建立測試人員風險管理原則。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-114">Create an insider risk management policy.</span></span>

<span data-ttu-id="8fbdb-115">如需有關測試人員風險原則如何協助您管理組織風險的詳細資訊，請參閱 [Microsoft 365 中的測試人員風險管理](https://go.microsoft.com/fwlink/?linkid=2123907)。</span><span class="sxs-lookup"><span data-stu-id="8fbdb-115">For more information about how insider risk polices can help you manage risk in your Organization, see [Insider risk management in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2123907).</span></span>
