---
title: 單一使用者的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428691"
---
# <a name="problem-with-single-user"></a><span data-ttu-id="b7214-102">單一使用者的問題</span><span class="sxs-lookup"><span data-stu-id="b7214-102">Problem with single user</span></span>

- <span data-ttu-id="b7214-103">使用者可能尚未布建，因為服務尚未有機會評估使用者。</span><span class="sxs-lookup"><span data-stu-id="b7214-103">The user may not have been provisioned because the service hasn't had a chance to evaluate the user yet.</span></span> <span data-ttu-id="b7214-104">在 [布建設定] 頁面上，回顧布建所需的時間和進度列的指導方針。</span><span class="sxs-lookup"><span data-stu-id="b7214-104">Review the guidance for how long provisioning takes as well as the progress bar on the provisioning configuration page.</span></span> <span data-ttu-id="b7214-105">如果 [其他詳細資料] 區段中所指定的穩定狀態是使用者建立/更新/刪除的日期，則表示尚未評估使用者。</span><span class="sxs-lookup"><span data-stu-id="b7214-105">If the steady state specified in the additional details section is before the date the user was created/updated/deleted, it means we have not evaluated the user yet.</span></span> <span data-ttu-id="b7214-106">在此案例中，最好的做法是等待布建服務完成。</span><span class="sxs-lookup"><span data-stu-id="b7214-106">In this scenario, the best thing to do is wait for the provisioning service to finish.</span></span>

  - <span data-ttu-id="b7214-107">請注意，我們的服務只會注意到來源系統中的使用者變更 (Cloud HR) 。</span><span class="sxs-lookup"><span data-stu-id="b7214-107">Note that our service is only aware of changes to a user in the source system (Cloud HR).</span></span> <span data-ttu-id="b7214-108">Azure AD 的來源系統中必須有有效的變更，才能偵測變更，並將其流式傳送至 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="b7214-108">There has to be a valid change in the source system for Azure AD to detect the change and flow it into Active Directory.</span></span>
- <span data-ttu-id="b7214-109">布建服務評估使用者並決定不應該布建：</span><span class="sxs-lookup"><span data-stu-id="b7214-109">Provisioning service evaluated the user and determined it should not be provisioned:</span></span>
  - <span data-ttu-id="b7214-110">如果您已設定屬性架構範圍篩選，請確定使用者符合您指定的準則。</span><span class="sxs-lookup"><span data-stu-id="b7214-110">If you have set an attribute based scoping filter, ensure that the user meets the criteria that you have specified.</span></span>
  - <span data-ttu-id="b7214-111">如果使用者已存在於目標系統中，且來源和目標中的使用者狀態為 [符合]，我們將不會採取任何進一步的動作。</span><span class="sxs-lookup"><span data-stu-id="b7214-111">If users already exist in the target system and the state of the user in the source and target match, we won't take any further action.</span></span>
- <span data-ttu-id="b7214-112">布建服務嘗試布建使用者，但失敗。</span><span class="sxs-lookup"><span data-stu-id="b7214-112">Provisioning service attempted to provision the user and it failed.</span></span> <span data-ttu-id="b7214-113">在這些案例中，請參閱布建記錄檔的疑難排解與建議] 索引標籤：</span><span class="sxs-lookup"><span data-stu-id="b7214-113">For these scenarios, review the troubleshooting and recommendations tab of the provisioning logs:</span></span>
  - <span data-ttu-id="b7214-114">在內部部署 Active Directory 或 Azure AD 中，使用者的必要屬性可能遺失。</span><span class="sxs-lookup"><span data-stu-id="b7214-114">A required attribute on the user might be missing in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="b7214-115">例如，userPrincipalName 或 sAMAccountName 產生規則不會產生正確的值。</span><span class="sxs-lookup"><span data-stu-id="b7214-115">For example, the userPrincipalName or sAMAccountName generation rules are not generating the right value.</span></span>
  - <span data-ttu-id="b7214-116">在內部部署 Active Directory 或 Azure AD 中，[) 公司單位] 的相符屬性 (通常不會解析為唯一的使用者。</span><span class="sxs-lookup"><span data-stu-id="b7214-116">The matching attribute (usually employeeId) is not resolving to a unique user in on-premises Active Directory or Azure AD.</span></span> <span data-ttu-id="b7214-117">例如，在 AD 中有兩位使用者有相同的雇員 Id，且該服務傳回錯誤碼，表示相同來源專案的重複目標專案。</span><span class="sxs-lookup"><span data-stu-id="b7214-117">For example, there are two users with the same employeeId in AD and the service returns an error code indicate duplicate target entries for the same source entry.</span></span>

<span data-ttu-id="b7214-118">若要查看單一使用者和群組的記錄，請參閱針對 [特定使用者的問題複查](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)布建記錄檔。</span><span class="sxs-lookup"><span data-stu-id="b7214-118">To review logs for single user and groups, see [Review the provisioning logs for an issue with a specific user](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).</span></span>
