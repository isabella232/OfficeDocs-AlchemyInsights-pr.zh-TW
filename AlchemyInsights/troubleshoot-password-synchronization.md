---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390402"
---
# <a name="troubleshoot-password-synchronization"></a>疑難排解密碼同步處理

若要疑難排解其中沒有密碼會同步處理與 Azure AD Connect 版本 1.1.614.0 或更新版本的問題：
  
1. 開啟新的 Windows PowerShell 工作階段，您的 Azure AD Connect 伺服器上具有 [**以管理員身分執行**] 選項。 
    
2. 執行**Set-executionpolicy RemoteSigned**或**Set-executionpolicy Unrestricted**。 
    
3. 啟動 Azure AD Connect 精靈。
    
4. 瀏覽至 [* * 其他工作 * *] 頁面上，選取 [* * 疑難排解 * *，按一下 [**下一步**。 
    
5. 在 [疑難排解] 頁面上，按一下**要啟動的疑難排解啟動**] 功能表 PowerShell 中。 
    
6. 在 [主要] 功能表中，選取**疑難排解密碼同步處理**。 
    
7. 子功能表中，選取 [**密碼同步處理未完全運作**。 
    
 **了解疑難排解工作的結果**
  
疑難排解工作會執行下列檢查：
  
- 驗證您的 Azure AD 租用戶，已啟用密碼同步處理功能。
    
- 驗證 Azure AD Connect 伺服器不在執行模式。
    
- 每個現有內部部署 Active Directory 連接器 （這會對應至現有的 Active Directory 樹系）：
    
- 
  - 驗證已啟用密碼同步處理功能。
    
  - 在 Windows 應用程式事件記錄檔的密碼同步處理活動訊號事件的搜尋。
    
  - 每個 Active Directory 網域下的內部部署 Active Directory 連接器：
    
  - 驗證的網域是可從 Azure AD Connect 伺服器。
    
  - 驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務 (AD DS) 帳戶具有正確的使用者名稱、 密碼及權限所需的密碼同步處理。
    
疑難排解密碼同步處理的詳細說明，請參閱[使用 Azure AD Connect 同步處理的疑難排解密碼同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。
  

