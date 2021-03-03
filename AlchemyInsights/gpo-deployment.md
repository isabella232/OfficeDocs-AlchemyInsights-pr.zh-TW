---
title: GPO 部署
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416938"
---
# <a name="gpo-deployment"></a><span data-ttu-id="3d2dd-102">GPO 部署</span><span class="sxs-lookup"><span data-stu-id="3d2dd-102">GPO Deployment</span></span>

<span data-ttu-id="3d2dd-103">Azure Active Directory Domain Services (Azure AD DS) 中使用者和電腦物件的設定通常是使用群組原則物件 (GPO) 進行管理。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-103">Settings for user and computer objects in Azure Active Directory Domain Services (Azure AD DS) are often managed using Group Policy Objects (GPOs).</span></span> <span data-ttu-id="3d2dd-104">Azure AD DS 包含內建 GPO，適用於 AADDC 使用者和 AADDC 電腦容器。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-104">Azure AD DS includes built-in GPOs for the AADDC Users and AADDC Computers containers.</span></span> <span data-ttu-id="3d2dd-105">您可以自訂這些內建 GPO，以便視環境需要設定群組原則。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-105">You can customize these built-in GPOs to configure group policy as needed for your environment.</span></span> <span data-ttu-id="3d2dd-106">Azure AD DC 系統管理員群組的成員擁有 Azure AD DS 網域中的群組原則管理權限，而且也能建立自訂 GPO 和組織單位 (OU)。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-106">Members of the Azure AD DC administrators group have group policy administration privileges in the Azure AD DS domain, and can also create custom GPOs and organizational units (OUs).</span></span> <span data-ttu-id="3d2dd-107">如需哪些群組原則及其運作方式的詳細資訊，請參閱 [群組原則一覽](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-107">For more information on what group policy is and how it works, see [Group Policy Overview](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).</span></span>

<span data-ttu-id="3d2dd-108">在混合式環境中，內部部署 AD DS 環境中設定的群組原則不會同步處理到 Azure AD DS。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-108">In a hybrid environment, group policies configured in an on-premises AD DS environment aren't synchronized to Azure AD DS.</span></span> <span data-ttu-id="3d2dd-109">若要在 Azure AD DS 中定義使用者或電腦的組態設定，請編輯其中一個預設 GPO，或建立自訂 GPO。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-109">To define configuration settings for users or computers in Azure AD DS, edit one of the default GPOs or create a custom GPO.</span></span>

<span data-ttu-id="3d2dd-110">本文《[管理群組原則](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy)》說明如何安裝群組原則管理工具、如何大量編輯內建的 GPO 以及如何建立自訂 GPO。</span><span class="sxs-lookup"><span data-stu-id="3d2dd-110">This article [Manage Group Policy](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) shows you how to install the Group Policy Management tools, how ton edit the built-in GPOs, and how to create custom GPOs.</span></span>
