---
title: 從 AIP 移轉至合規性中心的 MIP/統一標籤
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000347"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>從 AIP 移轉至合規性中心的 MIP/統一標籤

若要從 AIP 標籤移轉至安全性與合規性中心的統一標籤，請執行下列動作：

**從 Azure 入口網站啟用保護**

1. 如果您尚未這麼做，請開啟新的瀏覽器視窗，並[登入 Azure 入口網站](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal)。 瀏覽至 [Azure 資訊保護 **]** 刀鋒視窗。 例如，在中樞功能表上，按一下 [所有服務 **]**，然後在 [篩選] 方塊中開始輸入 **資訊**。 選取 [Azure 資訊保護 **]**。 如果您之前未存取過 [Azure 資訊保護] 刀鋒視窗，請參閱一次性的[額外步驟](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time)以將此刀鋒視窗新增至入口網站。 若要開啟 [Azure 資訊保護] 刀鋒視窗，您必須擁有 [Azure 資訊保護進階方案](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing)或包含版權管理的 Office 365 方案。 如果您擁有這其中一項訂閱，但看到訊息指出找不到有效的訂閱，請[連絡 Microsoft 支援服務](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support)，或使用您的標準支援通道。

2. 找到 [管理 **]** 功能表選項，然後選取 [保護啟用 **]**。 按一下 [啟用 **]**，然後確認您的動作。 啟用完成時，資訊列會顯示 [已成功完成啟動 **]**。

**將 Azure 資訊保護標籤移轉至 Office 365 安全性與合規性中心**

1. 確認您以具有全域系統管理員權限的使用者身分登入。

2. 瀏覽至 [Azure 資訊保護 **]** 刀鋒視窗。

3. 從 [管理 **]** 功能表選項，選取 [統一標籤 **]**。

4. 在 [Azure 資訊保護 - 統一標籤 **]** 刀鋒視窗上，按一下 [啟用 **]**，並遵循線上指示進行。

**注意**：請先驗證您擁有適當的權限，再啟動安全性與合規性中心移轉。如需詳細資訊，請參閱下列文章：

1. [必須是全域系統管理員才能設定 Azure 資訊保護，或者我可以委派給其他系統管理員嗎？](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [關於移轉至安全性與合規性中心之後，系統管理角色的重要資訊。](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

如需有關 AIP 移轉至安全性與合規性中心的統一標籤的詳細資訊，請參閱[移轉標籤](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)。
