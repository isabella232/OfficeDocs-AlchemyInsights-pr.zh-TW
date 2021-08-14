---
title: Privileged Identity Management 角色
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "6825"
ms.openlocfilehash: 358e446192e6b58ace81afa06e0d65ae3a207282351ffc3ec9975a24779951fb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973220"
---
# <a name="privileged-identity-managementpim-role"></a>Privileged Identity Management (PIM) 角色

**啟用角色之後未授與許可權**

當您在 Azure AD 中啟動角色時 Privileged Identity Management (PIM) ，啟用可能不會立即傳播至需要「特權」角色的所有入口網站。 有時候，即使變更遭到傳播，在入口網站中的 web 快取可能會導致變更不會立即生效。

如果您的啟用延遲，請遵循下列步驟：

1. 登出 Azure 入口網站，然後重新登入。 當您啟動 Azure AD 角色或 Azure 資源角色時，您將會看到您的啟用階段。 完成所有階段後，您將會看到「登出」連結。 您可以使用此連結登出。這會解決啟用延遲的大部分案例。
2. 在 PIM 中，確認您已列為該角色的成員。
3. 如果您要啟用 Exchange 系統管理員角色，請確定登出後再重新登入。 如果問題持續發生，請開啟支援票證，並將此問題當做問題提出。 如果您使用 Exchange 系統管理員角色來存取安全性與合規性中心，請參閱下一個步驟。
4. 如果您要啟用角色以存取安全性與合規性中心，或是若要啟用 SharePoint 系統管理員角色，您會在幾分鐘內經歷幾分鐘內的啟動延遲。 這是已知的問題，我們積極與這些小組合作，盡可能立即解決此問題。

如需詳細資訊，請參閱：

- [啟動我的 Azure AD role in PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?WT.mc_id=Portal-Microsoft_Azure_Support "HTTPs://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-activate-role?wt.mc_id=portal-microsoft_azure_support")
- [以 PIM 啟用我的 Azure 資源角色](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?WT.mc_id=Portal-Microsoft_Azure_Support "HTTPs://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-resource-roles-activate-your-roles?wt.mc_id=portal-microsoft_azure_support")

**停用角色或角色啟用到期後，不會移除許可權**

當您停用 Azure AD Privileged Identity Management 中的角色，或角色啟用期限到期時，可能會發生延遲，讓您繼續存取。

如果停用延遲，請遵循下列步驟：

1. 如果您要停用 Exchange 系統管理員角色或角色啟用期限到期，而且在移除許可權之前發現明顯的延遲，請開啟支援票證，並告知您的支援工程師，以協助您使用「許可權存取管理」 (PAM) 團隊內部 Office 關於此問題的相關資訊來處理票證。
2. 如果啟用期限已到期，但您仍已開啟瀏覽器會話，請關閉瀏覽器。 您可以繼續使用角色，直到您關閉該會話為止。 這是已知的問題，當啟用已到期時，我們就會查看每個會話的潛在修正會主動吊銷。

如果您的延遲與這兩個案例不同，請開啟支援票證。
