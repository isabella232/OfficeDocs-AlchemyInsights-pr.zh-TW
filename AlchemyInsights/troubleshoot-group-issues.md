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
# <a name="troubleshoot-group-issues"></a>疑難排解群組問題

**我需要為群組指派 Azure AD 角色**

若要為 Azure Active Directory (AD) 群組指 Azure AD 角色，請執行下列步驟：

1. 選立新群組 - 若要建立新的群組：

    a. 以特殊權限角色系統管理員或全域系統管理員權限登入 Azure AD 系統管理中心。 
    b. 選取 [Azure Active Directory] > [群組] > [所有群組] > [新增群組]。 
    c. 建立群組。

2. 在建立群組期間或建立群組之後，將角色指派給群組。

    a. 若要在建立群組時，將角色指派給群組，請切換 [可以將 Azure AD 角色指派給群組] 並建立群組。
    b. 若要在建立群組之後，將角色指派給該群組，請瀏覽至新建立群組的 [指派的角色] 索引標籤，然後將角色指派給群組。

**我需要管理獲派 Azure AD 角色的群組成員資格**

1. 為了防止提高權限，根據預設，只有特殊權限角色系統管理員和全域系統管理員可以修改指派給角色的群組成員資格。 不過，他們可以選擇為這類群組指派擁有者，並委派這個工作。 如需詳細資訊，請參閱[使用雲端群組來管理 Azure Active Directory 中的角色指派](https://docs.microsoft.com/azure/active-directory/roles/groups-concept) (部分機器翻譯)。
2. 如需在 Azure AD 中指派角色給群組的常見問題和疑難排解提示，請參閱[對指派給雲端群組的角色進行疑難排解](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting) (部分機器翻譯)。

**動態群組**

1. 如果您找不到內建的使用者屬性，請確定屬性位於支援的屬性清單中。
2. 如果您要尋找內建裝置屬性，請確定屬性位於裝置屬性清單中 
3. 除了內建的使用者和裝置屬性之外，您也可以使用[延伸模組屬性](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties)。 從內部部署 Windows Server AD 或連線的 SaaS 應用程式同步處理延伸模組屬性之後，屬性應該會顯示在規則建立器下拉式清單中。 您可以在目錄中找到自訂屬性名稱，方法為使用 PowerShell 查詢使用者的屬性並搜尋屬性名稱。 在規則語法中建構規則時，也可以使用這些屬性名稱。
4. 請確定您的租用戶擁有適當的授權。 動態群組要求租用戶擁有 Azure AD P1 進階版授權。 您可以在[這裡](https://azure.microsoft.com/pricing/details/active-directory/)取得 Azure AD 授權方案清單。 您可以在[這裡](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)取得 Enterprise Mobility + Security 授權方案。
5. 請確定建立動態群組的使用者角色是全域系統管理員、Intune 系統管理員、群組系統管理員或使用者系統管理員。
6. 請稍候，等待群組填入。 根據您的租用戶規模而定，群組第一次或規則變更後最多可能需要 24 小時才能填入。
7. 如需詳細資訊，請參閱[為動態群組成員資格建立屬性型規則](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership) (部分機器翻譯)。

**我需要刪除群組**

1. 您可以使用 Azure AD Powershell 模組中的 Remove-AzureADGroup Cmdlet 從目錄刪除群組。
2. 嘗試刪除 Azure AD 中已同步的群組之前，請先確認您已刪除所有指派的授權，以避免錯誤。
3. 如需刪除群組的詳細資訊，請參閱[刪除含指派授權的群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license) (部分機器翻譯)。

**我需要還原已刪除的群組​​**

1. 如果已刪除 Office 365 群組，必須在 30 天之內還原，之後則會永久刪除。 永久刪除之後，就無法再還原群組。 在[這裡](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)深入了解如何還原群組。
2. 安全性群組和通訊群組不支援此功能。
3. 請確定您擁有還原 Office 365 群組的授權。 全域系統管理員、群組系統管理員、使用者帳戶系統管理員、Intune 服務系統管理員、合作夥伴第 1 層或第 2 層支援，以及群組的擁有者都可以還原群組。
4. 刪除並還原動態群組後，它會被視為新群組，並依照規則重新填入。 可能需要 24 小時才能完成此程序。
5. 如需還原已刪除群組的詳細資訊，請參閱[還原 Azure Active Directory 中刪除的 Office 365 群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted) (部分機器翻譯)。

**群組到期原則設定**

1. 只有 Office 365 群組支援此功能，安全性群組和通訊群組不支援此功能。
2. 為 Office 365 群組設定和使用到期原則需要 Azure AD 進階版授權。
3. 目前，只能在租用戶上的 Office 365 群組設定一個到期原則。
4. 只有全域系統管理員、群組系統管理員、使用者系統管理員和群組擁有者才能更新群組。
5. 如果 Office 365 群組已到期，系統會將其刪除，必須在 30 天之內還原，之後則會永久刪除。 永久刪除之後，就無法再還原群組。 在[這裡](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)深入了解如何還原群組。

**活動型自動更新**

來自 SharePoint、Outlook 和 Teams 的使用者活動可觸發群組自動更新。 系統會在群組到期前 35 天檢查活動。 如果目前群組生命週期期間有活動，群組將會自動更新，且不會傳送電子郵件通知給群組擁有者。

**到期群組的通知時間**

1. 系統會在群組到期前 30 天、15 天和 1 天前，將電子郵件通知傳送給 Office 365 群組擁有者。
2. 當您第一次設定到期日時，任何超過到期時間的群組會設定為 35 天後到期。
3. 群組到期日是根據群組的更新日期計算，而不是根據原則更新日期計算。 如果更新到期原則，到期日將不會變更。
4. 如需詳細資訊，請參閱[群組到期原則和更新電子郵件](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle)和[在 Azure Active Directory 中還原已刪除的 Office 365 群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted) (部分機器翻譯)。

**建立群組的權限**

請確定您已獲得建立新群組的授權。 全域系統管理員可以在 Azure 入口網站或存取面板中停用群組建立。 您可能需要系統管理員才能建立新群組，或提供您適當權限。

1. [在 Azure 入口網站中建立新群組並新增成員](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [在 Powershell MSOnline 中建立群組](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [在 Powershell 中停用群組建立](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [管理能在 Office 365 中建立群組的使用者](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [透過 Powershell 停用 Office 365 歡迎通知](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Azure AD 系統管理員角色](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**管理群組建立權限**

1. 全域系統管理員可以在 Azure 入口網站設定的 [所有群組] > **[一般 (設定)]** 下，設定 **[使用者可在 Azure 入口網站中建立安全性群組]** 或 **[使用者可在 Azure 入口網站中建立 Office 365 群組]** 設定，管理在 Azure 入口網站或存取面板中建立之安全性或 Office 365 群組的群組建立權限。
2. 如果您擁有 Azure AD P1 進階版授權，也可以將群組建立限制為所選的一組使用者。

**停用 Office 365 群組新成員的歡迎通知**

在 Powershell 中將 `UnifiedGroupWelcomeMessageEnabled` 設定為 **False**，即可停止將歡迎通知傳送給新增至 Office 365 群組的使用者。 在[這裡](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)深入了解此設定。













