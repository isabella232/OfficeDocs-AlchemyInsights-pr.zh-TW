---
title: 多個使用者在 Outlook 中沒有看見增益集
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729862"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="39762-102">多個使用者在 Outlook 中沒有看見增益集</span><span class="sxs-lookup"><span data-stu-id="39762-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="39762-103">如果您測試 Outlook 增益集而其並未顯示出來，疑難排解步驟一，請使用 \*\*獲取-OrganizationConfig \*\* PowerShell Cmdlet 來查詢 _AppsForOfficeEnabled_ 參數。</span><span class="sxs-lookup"><span data-stu-id="39762-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="39762-104">如果查詢傳回 **[錯誤]** 值，請透過使用 **設定-OrganizationConfig** cmdlet 將參數設為 **[正確]**，這樣增益集就能正常顯示。</span><span class="sxs-lookup"><span data-stu-id="39762-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="39762-105">不建議將 _AppsForOfficeEnabled_ 參數設定為 **[錯誤]**。</span><span class="sxs-lookup"><span data-stu-id="39762-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="39762-106">**[錯誤]** 值會覆寫上述所有 [系統管理] 和 [使用者] 角色設定，並造成組織中的任何使用者無法啟用任何新的應用程式。</span><span class="sxs-lookup"><span data-stu-id="39762-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="39762-107">如需詳細資訊，請參閱[指定可安裝和管理 Outlook 增益集的系統管理員和使用者](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles)。</span><span class="sxs-lookup"><span data-stu-id="39762-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>