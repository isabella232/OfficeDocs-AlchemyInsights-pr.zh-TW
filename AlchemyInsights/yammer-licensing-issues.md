---
title: Yammer 授權問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657267"
---
# <a name="yammer-licensing-issues"></a>Yammer 授權問題

所有使用者都必須擁有使用 Yammer 企業版服務的授權，但根據預設，Yammer 不要求使用者需擁有存取服務的授權。 當系統管理員變更設定以封鎖沒有 Yammer 授權的 Microsoft 365 使用者時，未獲指派的 Yammer 企業版授權的使用者將無法存取 Yammer 服務。 如需詳細諮詢，請參閱 [在 Office 365 中管理 Yammer 使用者授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

當使用者的授權被移除時，將不再顯示 Yammer 選格，而其他服務可以使用授權移除來隱藏功能。 在其他情況下，仍然可以顯示功能，但需要授權指派才能運作。  

**授權尚未為使用者更新**  

有時候，儘管使用者已被指派授權，但仍無法存取 Yammer。 當有大量授權指派進行時，更有可能會發生延遲問題。 因為系統會以非同步方式執行，因此在 Azure AD 中，Yammer 使用者可能不會以變更的授權順序進行更新。 在開啟支援案例以報告授權同步處理問題之前，請等待24小時。  

**大量授權指派**  

您可以透過系統管理中心或 PowerShell 腳本編寫來指派授權。 如需詳細資訊，請參閱[指派授權給使用者](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)和[使用 Office 365 PowerShell 指派授權給使用者帳戶](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell)。 

Microsoft 支援服務不提供建立腳本的協助，但提供 Yammer 授權指派的文件。 如需詳細資訊，請參閱 [使用 Windows PowerShell 管理 Yammer 授權](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)。