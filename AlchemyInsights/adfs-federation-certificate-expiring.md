---
title: ADFS 同盟憑證到期
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662354"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 同盟憑證到期

若要解決此問題，請遵循下列步驟：
  
1. （如果尚未安裝模組） 的電腦上安裝 Microsoft Azure Active Directory 的 Windows PowerShell 模組。若要這樣做，前往[管理使用 Windows PowerShell 的 Azure AD](https://aka.ms/aadposh)。
    
2. 請遵循的步驟"案例 1： AD FS 權杖簽署憑證過期"] 區段中的[「 時發生問題存取的網站 」 從 AD FS 同盟的使用者登入 Office 365、 Azure、 或 Intune 時的錯誤](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。
    
3. 請遵循[如何更新或修復 Office 365、 Azure、 或 Intune 同盟網域的設定](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3)步驟。
    
    若要深入了解更新同盟憑證，請參閱[更新 Office 365 和 Azure Active Directory 的同盟憑證](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
    

