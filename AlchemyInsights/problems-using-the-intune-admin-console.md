---
title: 使用 Intune 系統管理員主控台時發生問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 10b37b2ffda50dc77396039a9e0e443ad81aef72
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728278"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="4f810-102">使用 Intune 系統管理員主控台時發生問題</span><span class="sxs-lookup"><span data-stu-id="4f810-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="4f810-103">**瀏覽 Intune 系統管理入口網站時「拒絕存取」。**</span><span class="sxs-lookup"><span data-stu-id="4f810-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="4f810-104">如果您是 Intune 自訂角色的成員，請確認您的帳戶已獲指派 Intune 或 Enterprise Mobility Suite (EMS) 授權。</span><span class="sxs-lookup"><span data-stu-id="4f810-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="4f810-105">如果您使用 Configuration Manager 管理裝置，請確認您不屬於 Configuration Manager MDM 的 Intune 使用者集合。</span><span class="sxs-lookup"><span data-stu-id="4f810-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="4f810-106">請確認您在 Intune 角色刀鋒視窗中已獲指派適當的角色型系統管理控制 (RBAC) 權限。</span><span class="sxs-lookup"><span data-stu-id="4f810-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="4f810-107">請確認使用的群組不是通訊群組清單。</span><span class="sxs-lookup"><span data-stu-id="4f810-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="4f810-108">Azure 入口網站中的 Intune 僅支援屬於 Azure Active Directory 安全性群組的使用者帳戶。</span><span class="sxs-lookup"><span data-stu-id="4f810-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="4f810-109">請檢閱 Azure 入口網站中的群組 > **[Intune]** > **[群組]**，或 Azure 入口網站 > **[Azure Active Directory]**。</span><span class="sxs-lookup"><span data-stu-id="4f810-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="4f810-110">**使用者對於獲指派的 Intune 角色擁有太多權限**</span><span class="sxs-lookup"><span data-stu-id="4f810-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="4f810-111">建議使用者移至 **[Intune]** > **[Intune 角色]** > **[我的權限]** > **[匯出]**，以檢閱獲授與的權限。</span><span class="sxs-lookup"><span data-stu-id="4f810-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="4f810-112">**我已將範圍群組新增至角色，但該角色的使用者仍然看得到其他使用者或裝置。**</span><span class="sxs-lookup"><span data-stu-id="4f810-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="4f810-113">範圍群組不會篩選出使用者或裝置。</span><span class="sxs-lookup"><span data-stu-id="4f810-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="4f810-114">範圍群組：</span><span class="sxs-lookup"><span data-stu-id="4f810-114">Scope groups:</span></span>

- <span data-ttu-id="4f810-115">限制使用者能夠指派原則或應用程式的對象。</span><span class="sxs-lookup"><span data-stu-id="4f810-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="4f810-116">只允許特定使用者在裝置上執行遠端工作。</span><span class="sxs-lookup"><span data-stu-id="4f810-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="4f810-117">如需有關範圍群組的詳細資訊，請參閱[使用 Microsoft Intune 的角色型存取控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。</span><span class="sxs-lookup"><span data-stu-id="4f810-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4f810-118">**我已經將使用者新增至 Intune 角色，但他們仍然擁有 Intune 系統管理員主控台的完整存取權。**</span><span class="sxs-lookup"><span data-stu-id="4f810-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="4f810-119">瀏覽至 Intune > Azure 入口網站中的 **[使用者]**，並確認使用者未獲指派 Azure 入口網站中的下列任何角色：</span><span class="sxs-lookup"><span data-stu-id="4f810-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="4f810-120">全域系統管理員</span><span class="sxs-lookup"><span data-stu-id="4f810-120">Global administrator</span></span>
- <span data-ttu-id="4f810-121">Intune 服務系統管理員</span><span class="sxs-lookup"><span data-stu-id="4f810-121">Intune service administrator</span></span>
- <span data-ttu-id="4f810-122">SharePoint 系統管理員</span><span class="sxs-lookup"><span data-stu-id="4f810-122">SharePoint administrator</span></span>

<span data-ttu-id="4f810-123">如需詳細資訊，請參閱[使用 Microsoft Intune 的角色型存取控制 (RBAC)](https://docs.microsoft.com/intune/role-based-access-control)。</span><span class="sxs-lookup"><span data-stu-id="4f810-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="4f810-124">**Access 問題**</span><span class="sxs-lookup"><span data-stu-id="4f810-124">**Access Issues**</span></span>

<span data-ttu-id="4f810-125">如需詳細資訊，請參閱[無法登入 Office 365、Azure 或 Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune)。</span><span class="sxs-lookup"><span data-stu-id="4f810-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>