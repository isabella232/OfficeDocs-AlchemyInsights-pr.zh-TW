---
title: 將群組指派給 Azure AD 角色
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/15/2021
ms.locfileid: "49875364"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="64e22-102">將群組指派給 Azure AD 角色</span><span class="sxs-lookup"><span data-stu-id="64e22-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="64e22-103">若要將 Azure AD 群組和 Azure AD 中的授權單位來源指派給 Azure AD 角色，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="64e22-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="64e22-104">選立新群組 - 若要建立新的群組：</span><span class="sxs-lookup"><span data-stu-id="64e22-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="64e22-105">a.</span><span class="sxs-lookup"><span data-stu-id="64e22-105">a.</span></span> <span data-ttu-id="64e22-106">以 **特殊權限角色管理員** 或 **全域系統管理員** 權限登入 Azure AD 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="64e22-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="64e22-107">b.</span><span class="sxs-lookup"><span data-stu-id="64e22-107">b.</span></span> <span data-ttu-id="64e22-108">選取 **[Azure Active Directory] > [群組] > [所有群組] > [新增群組]**。</span><span class="sxs-lookup"><span data-stu-id="64e22-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="64e22-109">c.</span><span class="sxs-lookup"><span data-stu-id="64e22-109">c.</span></span> <span data-ttu-id="64e22-110">建立群組。</span><span class="sxs-lookup"><span data-stu-id="64e22-110">Create the group.</span></span>

2. <span data-ttu-id="64e22-111">在建立群組期間或建立群組之後，將角色指派給群組。</span><span class="sxs-lookup"><span data-stu-id="64e22-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="64e22-112">a.</span><span class="sxs-lookup"><span data-stu-id="64e22-112">a.</span></span> <span data-ttu-id="64e22-113">若要在建立群組時，將角色指派給群組，請切換 **[可以將 Azure AD 角色指派給群組]** 並建立群組。</span><span class="sxs-lookup"><span data-stu-id="64e22-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="64e22-114">b.</span><span class="sxs-lookup"><span data-stu-id="64e22-114">b.</span></span> <span data-ttu-id="64e22-115">若要在建立群組之後，將角色指派給該群組，請瀏覽至新建立群組的 **[指派的角色]** 索引標籤，然後將角色指派給群組。</span><span class="sxs-lookup"><span data-stu-id="64e22-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="64e22-116">**管理指派給 Azure AD 角色的群組成員資格**</span><span class="sxs-lookup"><span data-stu-id="64e22-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="64e22-117">若要防止提高權限，根據預設，只有特殊權限管理員和全域系統管理員可以修改指派角色的群組成員資格。</span><span class="sxs-lookup"><span data-stu-id="64e22-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="64e22-118">不過，他們可以選擇指派群組的擁有者，並委派這個工作。</span><span class="sxs-lookup"><span data-stu-id="64e22-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="64e22-119">如需將雲端群組指派給 Azure AD 角色的詳細資訊，請參閱[將 AD 角色指派給雲端群組](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="64e22-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="64e22-120">如需疑難排解將角色指派給雲端群組的詳細資料，請參閱 [疑難排解將角色指派給雲端群組](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="64e22-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





