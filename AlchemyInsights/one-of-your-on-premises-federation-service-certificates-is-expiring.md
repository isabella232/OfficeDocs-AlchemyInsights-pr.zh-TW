---
title: 其中一個內部部署同盟服務憑證已過期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 9e2e1a1dd2993b2a02b4405db8a707b23ff4af16
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658898"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>其中一個內部部署同盟服務憑證已過期

若要解決此問題，請遵循下列步驟：
  
- （如果尚未安裝模組） 的電腦上安裝 Microsoft Azure Active Directory 的 Windows PowerShell 模組。若要這樣做，請移至[Azure Active Directory PowerShell 圖表](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- 請遵循的步驟"案例 1： AD FS 權杖簽署憑證過期"] 區段中的[「 時發生問題存取的網站 」 從 AD FS 同盟的使用者登入 Office 365、 Azure、 或 Intune 時的錯誤](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。
    
- 請遵循 t[如何更新或修復 Office 365、 Azure、 或 Intune 同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)步驟。
    
如需更新同盟憑證的詳細資訊，請參閱[O365 和 Azure AD 的憑證更新](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
  

