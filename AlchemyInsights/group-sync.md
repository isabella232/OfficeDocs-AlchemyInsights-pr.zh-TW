---
title: 群組同步
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/15/2021
ms.locfileid: "50243896"
---
# <a name="group-sync"></a><span data-ttu-id="e37d4-102">群組同步</span><span class="sxs-lookup"><span data-stu-id="e37d4-102">Group sync</span></span>

<span data-ttu-id="e37d4-103">本文提供群組同步的相關指導方針。</span><span class="sxs-lookup"><span data-stu-id="e37d4-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="e37d4-104">如果全域系統管理員或群組擁有者無法在 Azure 入口網站中修改群組屬性或新增成員或指派擁有者，請確認群組的授權來源為 Azure Active Directory (Azure AD)，全域系統管理員或群組擁有者才能修改該群組。</span><span class="sxs-lookup"><span data-stu-id="e37d4-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="e37d4-105">嘗試刪除 Azure AD 中已同步的群組之前，請先確認您已[刪除所有指派的授權](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced)，以避免錯誤。</span><span class="sxs-lookup"><span data-stu-id="e37d4-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="e37d4-106">若要了解如何同步使用者、群組和連絡人，請參閱 [Azure AD Connect 同步](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)，並遵循[使用 Azure AD Connect 將內部部署群組同步到 Azure](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) 的步驟，以使用 AD Connect 同步內部部署群組。</span><span class="sxs-lookup"><span data-stu-id="e37d4-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="e37d4-107">遵循此指南[疑難排解同步期間的錯誤](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors)，以疑難排解同步期間的常見錯誤。</span><span class="sxs-lookup"><span data-stu-id="e37d4-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

