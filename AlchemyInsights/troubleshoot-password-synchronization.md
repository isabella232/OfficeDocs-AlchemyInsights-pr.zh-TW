---
title: 疑難排解密碼同步處理
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105739"
---
# <a name="troubleshoot-password-synchronization"></a>疑難排解密碼同步處理

若要疑難排解密碼同步處理問題，請從使用此 AAD 連線疑難排解工作開始，以判斷密碼未同步處理的原因。 若要開始，請移至「 [管理直接同步](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)處理」。  

1. 在您的 Azure AD 連線伺服器上開啟新的 Windows PowerShell 會話，然後選取 [以 **系統管理員身分執行**] 選項。

2. 執行 Set-ExecutionPolicy RemoteSigned 或 Set-ExecutionPolicy 不限限制。

3. 啟動 Azure AD 連線嚮導。

4. 移至 [其他工作] 頁面 >**疑難排解**  >  **[下一步]**。

5. 選取 [ **啟動** ]，以開啟 [PowerShell 疑難排解] 功能表。

6. 選取 **[密碼同步處理疑難排解**]。

    此問題通常是不會同步處理特定使用者帳戶的密碼。

    **附注** 如果最後一次成功的密碼同步處理是一段時間，則密碼同步處理會失敗。

如需疑難排解密碼同步處理的詳細資訊，請參閱[使用 AZURE AD 連線 Sync 疑難排解密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)。