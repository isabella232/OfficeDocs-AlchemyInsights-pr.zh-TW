---
title: Workday 至 AD 使用者佈建進入隔離狀態
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
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430722"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="72e18-102">Workday 至 AD 使用者佈建進入隔離狀態</span><span class="sxs-lookup"><span data-stu-id="72e18-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="72e18-103">**Workday 至 AD 使用者佈建進入隔離狀態且 AD 中未建立使用者**</span><span class="sxs-lookup"><span data-stu-id="72e18-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="72e18-104">Workday 至 AD 使用者佈建工作進入隔離狀態，稽核記錄顯示匯出失敗事件，出現錯誤訊息 **錯誤：OperationsError-SvcErr：發生作業錯誤。尚未為目錄服務設定上層參照。目錄服務因此無法發行轉介給這個樹系外的物件**。</span><span class="sxs-lookup"><span data-stu-id="72e18-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="72e18-105">此錯誤通常在 Active Directory 容器 OU 未正確設定，或用於 **parentDistinguishedName** 的運算式對應發生問題時顯示。</span><span class="sxs-lookup"><span data-stu-id="72e18-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="72e18-106">檢查 **新使用者** 參數的預設 OU 是否輸入錯誤。</span><span class="sxs-lookup"><span data-stu-id="72e18-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="72e18-107">確保指定的 OU 已存在於您的 AD 中。</span><span class="sxs-lookup"><span data-stu-id="72e18-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="72e18-108">如果您在屬性對應中使用 **parentDistinguishedName**，請確保其一律評估為 AD 網域中的已知容器。</span><span class="sxs-lookup"><span data-stu-id="72e18-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="72e18-109">檢查稽核記錄中的匯出事件，以查看產生的值。</span><span class="sxs-lookup"><span data-stu-id="72e18-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="72e18-110">如需有關設定 Workday 以自動佈建的詳細資訊，請參閱[教學課程：設定 Workday 來自動佈建使用者](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)。</span><span class="sxs-lookup"><span data-stu-id="72e18-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

