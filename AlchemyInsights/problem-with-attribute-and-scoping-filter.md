---
title: 屬性和範圍篩選發生問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430724"
---
# <a name="problem-with-attribute-and-scoping-filter"></a><span data-ttu-id="baad6-102">屬性和範圍篩選發生問題</span><span class="sxs-lookup"><span data-stu-id="baad6-102">Problem with attribute and scoping filter</span></span>

<span data-ttu-id="baad6-103">**UPN 值衝突的問題**</span><span class="sxs-lookup"><span data-stu-id="baad6-103">**Issue with conflicting UPN values**</span></span>

<span data-ttu-id="baad6-104">Workday 至 AD 的使用者佈建顯示錯誤訊息 **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**。</span><span class="sxs-lookup"><span data-stu-id="baad6-104">The Workday to AD User Provisioning Workday to AD User Provisioning shows error message **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**.</span></span> <span data-ttu-id="baad6-105">作業失敗，因為針對新增/修改提供的 UPN 值並非全樹系唯一的值。</span><span class="sxs-lookup"><span data-stu-id="baad6-105">The operation failed because UPN value provided for addition/modification is not unique forest-wide.</span></span> <span data-ttu-id="baad6-106">錯誤詳細資料：**CONSTRAINT_ATT_TYPE - userPrincipalName**。</span><span class="sxs-lookup"><span data-stu-id="baad6-106">Error Details: **CONSTRAINT_ATT_TYPE - userPrincipalName**.</span></span>

<span data-ttu-id="baad6-107">目標 AD 網域已有建立 AD 使用者帳戶時 Workday 連接器嘗試設定的 **userPrincipalName** 值。</span><span class="sxs-lookup"><span data-stu-id="baad6-107">The **userPrincipalName** value that Workday connector is trying to set when creating the AD user account already exists in the target AD domain.</span></span> <span data-ttu-id="baad6-108">這表示 (1) 使用者已存在，且使用者的相符識別碼檢查失敗，或 (2) UPN 產生規則產生衝突值。</span><span class="sxs-lookup"><span data-stu-id="baad6-108">This implies that either (1) the user already exists and the matching ID check failed for the user or (2) the UPN generation rule generated a conflicting value.</span></span>

<span data-ttu-id="baad6-109">以下是建議解決方案的步驟：</span><span class="sxs-lookup"><span data-stu-id="baad6-109">Here are the suggested resolution steps:</span></span>

<span data-ttu-id="baad6-110">如果使用者已存在且相符識別碼檢查無法將 Workday 帳戶連結至 Active Directory 帳戶，請檢查 Workday 和 AD 中的相符識別碼屬性 (通常是 **employeeID**)是否完全相符。</span><span class="sxs-lookup"><span data-stu-id="baad6-110">If the user already exists and the matching ID check failed to link the Workday account to Active Directory account, then check if the matching ID attribute (typically **employeeID**) in both Workday and AD have an exact match.</span></span> <span data-ttu-id="baad6-111">如果不相符，這是需要修正的資料問題。</span><span class="sxs-lookup"><span data-stu-id="baad6-111">If they don't have a match, it is a data issue that needs to be fixed.</span></span> <span data-ttu-id="baad6-112">例如，如果 Workday 中的 EmployeeID 是 001052，而 AD 中的是 1052，則佈建引擎將無法連結這兩個帳戶，且會嘗試建立已存在的使用者。</span><span class="sxs-lookup"><span data-stu-id="baad6-112">For example, if the EmployeeID in Workday is 001052 and in AD it is 1052, then the provisioning engine will fail to link the two accounts and will try to create a user that already exists.</span></span> <span data-ttu-id="baad6-113">此案例中的解決方案是將 AD 中的 **EmployeeID** 值變更為包含前置數字零，即為 001052。</span><span class="sxs-lookup"><span data-stu-id="baad6-113">The solution in this case is to change the **EmployeeID** value in AD to include the leading zeros to make it 001052.</span></span>
<span data-ttu-id="baad6-114">如果 UPN 產生的運算式未產生唯一值，請考慮使用重複資料刪除功能 **SelectUniqueValue**，以每次皆產生唯一值。</span><span class="sxs-lookup"><span data-stu-id="baad6-114">If the UPN-generating expression is not generating a unique value, consider using the de-duplication function **SelectUniqueValue** to generate a unique value each time.</span></span>

<span data-ttu-id="baad6-115">**Workday 至 AD 的使用者佈建未設定 AD 使用者帳戶的管理員屬性值**</span><span class="sxs-lookup"><span data-stu-id="baad6-115">**Workday to AD User Provisioning does not set manager attribute value for AD user account**</span></span>

<span data-ttu-id="baad6-116">Workday 至 AD 的使用者佈建工作未設定 AD 使用者帳戶的 **管理員** 屬性值。</span><span class="sxs-lookup"><span data-stu-id="baad6-116">The Workday to AD User Provisioning job is not setting the **manager** attribute value for AD user accounts.</span></span> <span data-ttu-id="baad6-117">出現此行為時，有兩種可能的情況：</span><span class="sxs-lookup"><span data-stu-id="baad6-117">There are two possible scenarios when this behavior is seen:</span></span>

1. <span data-ttu-id="baad6-118">無法將 Workday 中的管理員解析為對應的 AD 使用者帳戶，因為該管理員不在範圍內。</span><span class="sxs-lookup"><span data-stu-id="baad6-118">The manager in Workday cannot be resolved to a corresponding AD User account because the manager is not in scope.</span></span>
2. <span data-ttu-id="baad6-119">在 **多個 AD 網域** 情況中，Workday 中的管理員與使用者不在相同網域中。</span><span class="sxs-lookup"><span data-stu-id="baad6-119">In a **multiple AD domains** scenario, the manager in Workday is not present in the same domain as the user.</span></span>

<span data-ttu-id="baad6-120">請嘗試下列步驟以解決問題：</span><span class="sxs-lookup"><span data-stu-id="baad6-120">Try these steps to resolve the issue:</span></span>

1. <span data-ttu-id="baad6-121">如果您已定義範圍篩選，請先檢查管理員是否位於範圍內且滿足範圍子句。</span><span class="sxs-lookup"><span data-stu-id="baad6-121">If you have defined scoping filters, first check if the manager is in scope and that it satisfies the scoping clause.</span></span> <span data-ttu-id="baad6-122">如果管理員不符合範圍篩選準則，請變更篩選器，使管理員也位於佈建作業的範圍內。</span><span class="sxs-lookup"><span data-stu-id="baad6-122">If the manager does not satisfy the scoping filter, change the filter so that the manager is also in scope of the provisioning operation.</span></span>
2. <span data-ttu-id="baad6-123">如果您有多個 AD 網域，則連接器具有已知的限制，即為無法解析跨網域管理員參照。</span><span class="sxs-lookup"><span data-stu-id="baad6-123">If you have multiple AD domains, then the connector has a known limitation of inability to resolve cross-domain manager references.</span></span>

<span data-ttu-id="baad6-124">如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="baad6-124">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>













