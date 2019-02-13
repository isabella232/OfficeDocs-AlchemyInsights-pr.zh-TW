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
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924687"
---
# <a name="troubleshoot-password-synchronization"></a>疑難排解密碼同步處理

若要疑難排解其中沒有密碼會與 Azure AD 連接版本 1.1.614.0 同步處理或更新版本的問題：
  
1. 開啟新的 Windows PowerShell 工作階段 Azure AD 連線伺服器上使用 [**以系統管理員身分執行**] 選項。 
    
2. 執行**Set-executionpolicy RemoteSigned**或**Set-executionpolicy Unrestricted**。 
    
3. 啟動 Azure AD 連線精靈]。
    
4. 瀏覽至 [* * 其他工作 * *] 頁面上，選取 [* * Troubleshoot * *，然後按一下 [**下一步**。 
    
5. 疑難排解] 索引標籤上按一下 [**啟動疑難排解啟動**] 功能表中使用 PowerShell。 
    
6. 在 [主要] 功能表中選取 [**疑難排解密碼同步處理**]。 
    
7. 子功能表中選取 [**密碼同步處理未完全運作**。 
    
 **了解疑難排解工作的結果**
  
疑難排解工作會執行下列檢查：
  
- 驗證的密碼同步處理功能已啟用 Azure AD 租用。
    
- 驗證 Azure AD 連線伺服器不是在執行模式。
    
- 每個現有內部部署 Active Directory 連接器 （這會對應至現有的 Active Directory 樹系）：
    
- 
  - 驗證已啟用密碼同步處理功能。
    
  - 搜尋的 Windows 應用程式事件記錄檔中的密碼同步處理活動訊號事件。
    
  - 每個 Active Directory 網域的內部部署 Active Directory 連接器底下：
    
  - 驗證網域可從 Azure AD 連線伺服器。
    
  - 驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務 (AD DS) 帳戶具有正確的使用者名稱、 密碼和密碼同步處理所需的權限。
    
密碼同步處理的疑難排解的詳細說明，請參閱 ＜ [Troubleshoot 密碼同步處理 Azure AD 連線同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。
  

