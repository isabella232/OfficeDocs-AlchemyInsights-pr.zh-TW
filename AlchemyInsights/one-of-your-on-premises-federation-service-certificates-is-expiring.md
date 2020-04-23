---
title: 您的其中一個內部部署同盟服務憑證已過期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: dafa344ec649002900e98a5e183b3e5f759707e1
ms.sourcegitcommit: 6a3748f5c05693ca0c19a829287cb8f30635940c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43785294"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>您的其中一個內部部署同盟服務憑證已過期

若要解決此問題，請遵循下列步驟：
  
- 在電腦上安裝 Windows PowerShell 的 Microsoft Azure Active Directory 模組（如果尚未安裝模組）。 若要這麼做，請移至[Azure Active Directory PowerShell 的圖形](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 請遵循「案例1： AD FS 權杖簽署憑證已過期」一節中的「案例」[當同盟使用者登入 Microsoft 365、Azure 或 Intune 時，「存取網站時發生問題](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)」一節。
    
- 請依照[如何更新或修復 Microsoft 365、Azure 或 Intune 中的同盟網域設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)中的步驟進行。
    
如需有關如何更新同盟憑證的詳細資訊，請參閱[用於 O365 和 AZURE AD 的憑證更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
  

