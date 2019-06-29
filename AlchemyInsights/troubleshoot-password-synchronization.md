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
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353096"
---
# <a name="troubleshoot-password-synchronization"></a>疑難排解密碼同步處理

若要疑難排解與 Azure AD Connect 版本1.1.614.0 或更新版本不同步的密碼, 請執行下列動作:
  
1. 使用 [以**系統管理員身分執行**] 選項, 在 Azure AD Connect 伺服器上開啟新的 Windows PowerShell 會話。

2. 執行**ExecutionPolicy RemoteSigned**或**Set-ExecutionPolicy 無限制**。

3. 啟動 Azure AD Connect 嚮導。

4. 流覽至 [**其他**工作] 頁面, 選取 [**疑難排解**], 然後按 **[下一步]**。

5. 在 [疑難排解] 頁面上, 按一下 [啟動],**以啟動 PowerShell 中的疑難排解**功能表。

6. 在主功能表中, 選取 [**疑難排解密碼同步**處理]。

7. 在 [子功能表] 中, 選取 [**密碼同步處理] 根本無法運作**。

**瞭解疑難排解工作的結果**
  
疑難排解工作會執行下列檢查:
  
- 驗證您的 Azure AD 租使用者已啟用密碼同步處理功能。

- 驗證 Azure AD Connect 伺服器不在分段模式中。

- 針對每個現有的內部部署 Active Directory 連接器 (對應至現有的 Active Directory 樹系):

- 
  - 驗證是否已啟用密碼同步處理功能。

  - 在 Windows 應用程式事件記錄檔中搜尋密碼同步處理心跳事件。

  - 針對內部部署 Active Directory 連接器底下的每個 Active Directory 網域:

  - 驗證網域是否可從 Azure AD Connect 伺服器存取。

  - 驗證內部部署 Active Directory 連接器所使用的 Active Directory 網域服務 (AD DS) 帳戶是否有正確的使用者名稱、密碼, 以及密碼同步處理所需的許可權。

如需疑難排解密碼同步處理的詳細資訊, 請參閱[使用 AZURE AD Connect Sync 疑難排解密碼同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)。
  