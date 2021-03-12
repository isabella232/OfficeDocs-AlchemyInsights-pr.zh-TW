---
title: 疑難排解群組問題
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
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "50716104"
---
# <a name="troubleshoot-group-issues"></a><span data-ttu-id="c27f3-102">疑難排解群組問題</span><span class="sxs-lookup"><span data-stu-id="c27f3-102">Troubleshoot group issues</span></span>

<span data-ttu-id="c27f3-103">**我需要為群組指派 Azure AD 角色**</span><span class="sxs-lookup"><span data-stu-id="c27f3-103">**I need to assign a group to an Azure AD role**</span></span>

<span data-ttu-id="c27f3-104">若要為 Azure Active Directory (AD) 群組指 Azure AD 角色，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="c27f3-104">To assign an Azure Active Directory (AD) group to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="c27f3-105">選立新群組 - 若要建立新的群組：</span><span class="sxs-lookup"><span data-stu-id="c27f3-105">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="c27f3-106">a.</span><span class="sxs-lookup"><span data-stu-id="c27f3-106">a.</span></span> <span data-ttu-id="c27f3-107">以特殊權限角色系統管理員或全域系統管理員權限登入 Azure AD 系統管理中心。</span><span class="sxs-lookup"><span data-stu-id="c27f3-107">Sign in to the Azure AD admin center with privileged role administrator or global administrator permissions.</span></span> 
    <span data-ttu-id="c27f3-108">b.</span><span class="sxs-lookup"><span data-stu-id="c27f3-108">b.</span></span> <span data-ttu-id="c27f3-109">選取 [Azure Active Directory] > [群組] > [所有群組] > [新增群組]。</span><span class="sxs-lookup"><span data-stu-id="c27f3-109">Select Azure Active Directory > Groups > All groups > New group.</span></span> 
    <span data-ttu-id="c27f3-110">c.</span><span class="sxs-lookup"><span data-stu-id="c27f3-110">c.</span></span> <span data-ttu-id="c27f3-111">建立群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-111">Create the group.</span></span>

2. <span data-ttu-id="c27f3-112">在建立群組期間或建立群組之後，將角色指派給群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-112">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="c27f3-113">a.</span><span class="sxs-lookup"><span data-stu-id="c27f3-113">a.</span></span> <span data-ttu-id="c27f3-114">若要在建立群組時，將角色指派給群組，請切換 [可以將 Azure AD 角色指派給群組] 並建立群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-114">To assign a role to the group at the time of group creation, switch on the toggle Azure AD roles can be assigned to the group and create the group.</span></span>
    <span data-ttu-id="c27f3-115">b.</span><span class="sxs-lookup"><span data-stu-id="c27f3-115">b.</span></span> <span data-ttu-id="c27f3-116">若要在建立群組之後，將角色指派給該群組，請瀏覽至新建立群組的 [指派的角色] 索引標籤，然後將角色指派給群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-116">To assign a role to the group after it has been created, navigate to the Assigned roles tab for the newly created group, and assign the role to the group.</span></span>

<span data-ttu-id="c27f3-117">**我需要管理獲派 Azure AD 角色的群組成員資格**</span><span class="sxs-lookup"><span data-stu-id="c27f3-117">**I need to manage membership of a group that is assigned to Azure AD role**</span></span>

1. <span data-ttu-id="c27f3-118">為了防止提高權限，根據預設，只有特殊權限角色系統管理員和全域系統管理員可以修改指派給角色的群組成員資格。</span><span class="sxs-lookup"><span data-stu-id="c27f3-118">To prevent elevation of privileges, by default, only privileged role administrator and global administrator can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="c27f3-119">不過，他們可以選擇為這類群組指派擁有者，並委派這個工作。</span><span class="sxs-lookup"><span data-stu-id="c27f3-119">They can, however, choose to assign an owner for such a group and delegate this task.</span></span> <span data-ttu-id="c27f3-120">如需詳細資訊，請參閱[使用雲端群組來管理 Azure Active Directory 中的角色指派](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-120">For more information see, [Use cloud groups to manage role assignments in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span>
2. <span data-ttu-id="c27f3-121">如需在 Azure AD 中指派角色給群組的常見問題和疑難排解提示，請參閱[對指派給雲端群組的角色進行疑難排解](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-121">For common questions and troubleshooting tips for assigning roles to groups in Azure AD, see [Troubleshooting roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>

<span data-ttu-id="c27f3-122">**動態群組**</span><span class="sxs-lookup"><span data-stu-id="c27f3-122">**Dynamic groups**</span></span>

1. <span data-ttu-id="c27f3-123">如果您找不到內建的使用者屬性，請確定屬性位於支援的屬性清單中。</span><span class="sxs-lookup"><span data-stu-id="c27f3-123">If you cannot find the built-in user attributes, ensure that the attribute is in the list of supported properties.</span></span>
2. <span data-ttu-id="c27f3-124">如果您要尋找內建裝置屬性，請確定屬性位於裝置屬性清單中</span><span class="sxs-lookup"><span data-stu-id="c27f3-124">If you are looking for built-in device attributes, ensure that the attribute is in the list of device attributes</span></span> 
3. <span data-ttu-id="c27f3-125">除了內建的使用者和裝置屬性之外，您也可以使用[延伸模組屬性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-125">In addition to the built-in user and device attributes, you could also use [Extension Attributes](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties).</span></span> <span data-ttu-id="c27f3-126">從內部部署 Windows Server AD 或連線的 SaaS 應用程式同步處理延伸模組屬性之後，屬性應該會顯示在規則建立器下拉式清單中。</span><span class="sxs-lookup"><span data-stu-id="c27f3-126">After syncing extension attributes from on-premises Windows Server AD or from a connected SaaS application, the attributes should be visible in the drop-down list of the rule builder.</span></span> <span data-ttu-id="c27f3-127">您可以在目錄中找到自訂屬性名稱，方法為使用 PowerShell 查詢使用者的屬性並搜尋屬性名稱。</span><span class="sxs-lookup"><span data-stu-id="c27f3-127">The custom attribute name can be found in the directory by querying a user's attribute using PowerShell and searching for the attribute name.</span></span> <span data-ttu-id="c27f3-128">在規則語法中建構規則時，也可以使用這些屬性名稱。</span><span class="sxs-lookup"><span data-stu-id="c27f3-128">These could also be used when constructing rules in the rule syntax.</span></span>
4. <span data-ttu-id="c27f3-129">請確定您的租用戶擁有適當的授權。</span><span class="sxs-lookup"><span data-stu-id="c27f3-129">Ensure that your tenant has the appropriate license.</span></span> <span data-ttu-id="c27f3-130">動態群組要求租用戶擁有 Azure AD P1 進階版授權。</span><span class="sxs-lookup"><span data-stu-id="c27f3-130">Dynamic groups require the tenant to have an Azure AD P1 Premium license.</span></span> <span data-ttu-id="c27f3-131">您可以在[這裡](https://azure.microsoft.com/pricing/details/active-directory/)取得 Azure AD 授權方案清單。</span><span class="sxs-lookup"><span data-stu-id="c27f3-131">The list of Azure AD license plans can be accessed [here](https://azure.microsoft.com/pricing/details/active-directory/).</span></span> <span data-ttu-id="c27f3-132">您可以在[這裡](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)取得 Enterprise Mobility + Security 授權方案。</span><span class="sxs-lookup"><span data-stu-id="c27f3-132">Enterprise Mobility + Security licensing plans can be accessed [here](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing).</span></span>
5. <span data-ttu-id="c27f3-133">請確定建立動態群組的使用者角色是全域系統管理員、Intune 系統管理員、群組系統管理員或使用者系統管理員。</span><span class="sxs-lookup"><span data-stu-id="c27f3-133">Ensure that the role of the user creating the dynamic group is a global administrator, intune administrator, group administrator, or a user administrator.</span></span>
6. <span data-ttu-id="c27f3-134">請稍候，等待群組填入。</span><span class="sxs-lookup"><span data-stu-id="c27f3-134">Please allow time for the group to populate.</span></span> <span data-ttu-id="c27f3-135">根據您的租用戶規模而定，群組第一次或規則變更後最多可能需要 24 小時才能填入。</span><span class="sxs-lookup"><span data-stu-id="c27f3-135">Depending on the size of your tenant, the group may take up to 24 hours for populating for the first time or after a rule change.</span></span>
7. <span data-ttu-id="c27f3-136">如需詳細資訊，請參閱[為動態群組成員資格建立屬性型規則](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-136">For more information, see [Create attribute-based rules for dynamic group membership](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership).</span></span>

<span data-ttu-id="c27f3-137">**我需要刪除群組**</span><span class="sxs-lookup"><span data-stu-id="c27f3-137">**I need to delete a group**</span></span>

1. <span data-ttu-id="c27f3-138">您可以使用 Azure AD Powershell 模組中的 Remove-AzureADGroup Cmdlet 從目錄刪除群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-138">Groups can be deleted from the directory using the Remove-AzureADGroup cmdlet in the Azure AD Powershell module.</span></span>
2. <span data-ttu-id="c27f3-139">嘗試刪除 Azure AD 中已同步的群組之前，請先確認您已刪除所有指派的授權，以避免錯誤。</span><span class="sxs-lookup"><span data-stu-id="c27f3-139">Before attempting to delete a synced group in Azure AD, ensure you have deleted all assigned licenses  to avoid errors.</span></span>
3. <span data-ttu-id="c27f3-140">如需刪除群組的詳細資訊，請參閱[刪除含指派授權的群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-140">For more information on deleting groups, see [Deleting a group with an assigned license](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license).</span></span>

<span data-ttu-id="c27f3-141">**我需要還原已刪除的群組​​**</span><span class="sxs-lookup"><span data-stu-id="c27f3-141">**I need to restore a deleted group**</span></span>

1. <span data-ttu-id="c27f3-142">如果已刪除 Office 365 群組，必須在 30 天之內還原，之後則會永久刪除。</span><span class="sxs-lookup"><span data-stu-id="c27f3-142">If an Office 365 group is deleted, it can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="c27f3-143">永久刪除之後，就無法再還原群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-143">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="c27f3-144">在[這裡](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)深入了解如何還原群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-144">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>
2. <span data-ttu-id="c27f3-145">安全性群組和通訊群組不支援此功能。</span><span class="sxs-lookup"><span data-stu-id="c27f3-145">This functionality is not supported for security groups and distribution groups.</span></span>
3. <span data-ttu-id="c27f3-146">請確定您擁有還原 Office 365 群組的授權。</span><span class="sxs-lookup"><span data-stu-id="c27f3-146">Ensure you are authorized to restore an Office 365 group.</span></span> <span data-ttu-id="c27f3-147">全域系統管理員、群組系統管理員、使用者帳戶系統管理員、Intune 服務系統管理員、合作夥伴第 1 層或第 2 層支援，以及群組的擁有者都可以還原群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-147">Global administrators, group administrators, user account administrators, intune service administrators, partner tier1 or tier2 support, and the owner of the group can be able to restore a group.</span></span>
4. <span data-ttu-id="c27f3-148">刪除並還原動態群組後，它會被視為新群組，並依照規則重新填入。</span><span class="sxs-lookup"><span data-stu-id="c27f3-148">When a dynamic group is deleted and restored, it is seen as a new group and re-populated according to the rule.</span></span> <span data-ttu-id="c27f3-149">可能需要 24 小時才能完成此程序。</span><span class="sxs-lookup"><span data-stu-id="c27f3-149">This process might take up to 24 hours.</span></span>
5. <span data-ttu-id="c27f3-150">如需還原已刪除群組的詳細資訊，請參閱[還原 Azure Active Directory 中刪除的 Office 365 群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-150">For more information on restoring a deleted group, see [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c27f3-151">**群組到期原則設定**</span><span class="sxs-lookup"><span data-stu-id="c27f3-151">**Group expiration policy configuration**</span></span>

1. <span data-ttu-id="c27f3-152">只有 Office 365 群組支援此功能，安全性群組和通訊群組不支援此功能。</span><span class="sxs-lookup"><span data-stu-id="c27f3-152">This functionality is only supported for Office 365 groups, and not for security groups and distribution groups are not supported.</span></span>
2. <span data-ttu-id="c27f3-153">為 Office 365 群組設定和使用到期原則需要 Azure AD 進階版授權。</span><span class="sxs-lookup"><span data-stu-id="c27f3-153">Configuring and using the expiration policy for Office 365 groups requires an Azure AD Premium license.</span></span>
3. <span data-ttu-id="c27f3-154">目前，只能在租用戶上的 Office 365 群組設定一個到期原則。</span><span class="sxs-lookup"><span data-stu-id="c27f3-154">Currently, only one expiration policy can be configured for Office 365 groups on a tenant.</span></span>
4. <span data-ttu-id="c27f3-155">只有全域系統管理員、群組系統管理員、使用者系統管理員和群組擁有者才能更新群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-155">Only Global administrators, group administrators, user administrators, and the owner of the group can be able to renew a group.</span></span>
5. <span data-ttu-id="c27f3-156">如果 Office 365 群組已到期，系統會將其刪除，必須在 30 天之內還原，之後則會永久刪除。</span><span class="sxs-lookup"><span data-stu-id="c27f3-156">If an Office 365 group is expired, it is deleted and can only be restored up to 30 days before permanent deletion occurs.</span></span> <span data-ttu-id="c27f3-157">永久刪除之後，就無法再還原群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-157">Once permanently deleted, the group can no longer be restored.</span></span> <span data-ttu-id="c27f3-158">在[這裡](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)深入了解如何還原群組。</span><span class="sxs-lookup"><span data-stu-id="c27f3-158">Learn more about restoring groups [here](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c27f3-159">**活動型自動更新**</span><span class="sxs-lookup"><span data-stu-id="c27f3-159">**Activity-based automatic renewal**</span></span>

<span data-ttu-id="c27f3-160">來自 SharePoint、Outlook 和 Teams 的使用者活動可觸發群組自動更新。</span><span class="sxs-lookup"><span data-stu-id="c27f3-160">User activities from SharePoint, Outlook and Teams can trigger group automatic renewal.</span></span> <span data-ttu-id="c27f3-161">系統會在群組到期前 35 天檢查活動。</span><span class="sxs-lookup"><span data-stu-id="c27f3-161">Activities are checked at 35 days before a group expires.</span></span> <span data-ttu-id="c27f3-162">如果目前群組生命週期期間有活動，群組將會自動更新，且不會傳送電子郵件通知給群組擁有者。</span><span class="sxs-lookup"><span data-stu-id="c27f3-162">If there is activity during the current group lifecycle, the group will be automatically renewed and email notification won't be sent out to group owners.</span></span>

<span data-ttu-id="c27f3-163">**到期群組的通知時間**</span><span class="sxs-lookup"><span data-stu-id="c27f3-163">**Notification timing for expired groups**</span></span>

1. <span data-ttu-id="c27f3-164">系統會在群組到期前 30 天、15 天和 1 天前，將電子郵件通知傳送給 Office 365 群組擁有者。</span><span class="sxs-lookup"><span data-stu-id="c27f3-164">Email notifications are sent to the Office 365 group owners 30 days, 15 days, and 1 day prior to expiration of the group.</span></span>
2. <span data-ttu-id="c27f3-165">當您第一次設定到期日時，任何超過到期時間的群組會設定為 35 天後到期。</span><span class="sxs-lookup"><span data-stu-id="c27f3-165">When you first set up expiration, any groups that are older than the expiration interval are set to 35 days until expiration.</span></span>
3. <span data-ttu-id="c27f3-166">群組到期日是根據群組的更新日期計算，而不是根據原則更新日期計算。</span><span class="sxs-lookup"><span data-stu-id="c27f3-166">Group expiration date is calculated based on the group’s renewal date, not based on the policy updated date.</span></span> <span data-ttu-id="c27f3-167">如果更新到期原則，到期日將不會變更。</span><span class="sxs-lookup"><span data-stu-id="c27f3-167">If the expiration policy is updated, the expiration date will not change.</span></span>
4. <span data-ttu-id="c27f3-168">如需詳細資訊，請參閱[群組到期原則和更新電子郵件](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle)和[在 Azure Active Directory 中還原已刪除的 Office 365 群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="c27f3-168">For more information see, [Group Expiration policy and renewal emails](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) and [Restore a deleted Office 365 group in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted).</span></span>

<span data-ttu-id="c27f3-169">**建立群組的權限**</span><span class="sxs-lookup"><span data-stu-id="c27f3-169">**Permission to create a group**</span></span>

<span data-ttu-id="c27f3-170">請確定您已獲得建立新群組的授權。</span><span class="sxs-lookup"><span data-stu-id="c27f3-170">Ensure that you are authorized to create a new group.</span></span> <span data-ttu-id="c27f3-171">全域系統管理員可以在 Azure 入口網站或存取面板中停用群組建立。</span><span class="sxs-lookup"><span data-stu-id="c27f3-171">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="c27f3-172">您可能需要系統管理員才能建立新群組，或提供您適當權限。</span><span class="sxs-lookup"><span data-stu-id="c27f3-172">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

1. [<span data-ttu-id="c27f3-173">在 Azure 入口網站中建立新群組並新增成員</span><span class="sxs-lookup"><span data-stu-id="c27f3-173">Create a new group and add members in Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [<span data-ttu-id="c27f3-174">在 Powershell MSOnline 中建立群組</span><span class="sxs-lookup"><span data-stu-id="c27f3-174">Create groups in Powershell MSOnline</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [<span data-ttu-id="c27f3-175">在 Powershell 中停用群組建立</span><span class="sxs-lookup"><span data-stu-id="c27f3-175">Disable groups creation in Powershell</span></span>](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [<span data-ttu-id="c27f3-176">管理能在 Office 365 中建立群組的使用者</span><span class="sxs-lookup"><span data-stu-id="c27f3-176">Manage who can create groups in Office 365</span></span>](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [<span data-ttu-id="c27f3-177">透過 Powershell 停用 Office 365 歡迎通知</span><span class="sxs-lookup"><span data-stu-id="c27f3-177">Disable Office 365 welcome notification via Powershell</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [<span data-ttu-id="c27f3-178">Azure AD 系統管理員角色</span><span class="sxs-lookup"><span data-stu-id="c27f3-178">Azure AD administrative roles</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

<span data-ttu-id="c27f3-179">**管理群組建立權限**</span><span class="sxs-lookup"><span data-stu-id="c27f3-179">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="c27f3-180">全域系統管理員可以在 Azure 入口網站設定的 [所有群組] > **[一般 (設定)]** 下，設定 **[使用者可在 Azure 入口網站中建立安全性群組]** 或 **[使用者可在 Azure 入口網站中建立 Office 365 群組]** 設定，管理在 Azure 入口網站或存取面板中建立之安全性或 Office 365 群組的群組建立權限。</span><span class="sxs-lookup"><span data-stu-id="c27f3-180">Global administrators can manage group creation permissions for security or Office 365 groups created in the Azure portal or Access Panel, by setting **Users can create security groups in Azure portals** or **Users can create Office 365 groups in Azure portals** settings in **All groups > General (Settings)**.</span></span>
2. <span data-ttu-id="c27f3-181">如果您擁有 Azure AD P1 進階版授權，也可以將群組建立限制為所選的一組使用者。</span><span class="sxs-lookup"><span data-stu-id="c27f3-181">You can also restrict group creation to select a group of users if you have an Azure AD P1 Premium license.</span></span>

<span data-ttu-id="c27f3-182">**停用 Office 365 群組新成員的歡迎通知**</span><span class="sxs-lookup"><span data-stu-id="c27f3-182">**Disabling welcome notification for new members of an Office 365 group**</span></span>

<span data-ttu-id="c27f3-183">在 Powershell 中將 `UnifiedGroupWelcomeMessageEnabled` 設定為 **False**，即可停止將歡迎通知傳送給新增至 Office 365 群組的使用者。</span><span class="sxs-lookup"><span data-stu-id="c27f3-183">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting `UnifiedGroupWelcomeMessageEnabled` to **False** in Powershell.</span></span> <span data-ttu-id="c27f3-184">在[這裡](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)深入了解此設定。</span><span class="sxs-lookup"><span data-stu-id="c27f3-184">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup).</span></span>













