---
title: 疑難排解用戶端驗證憑證部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509043"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>疑難排解用戶端驗證憑證部署

Intune NDES/SCEP 和 PKCS/PFX 用戶端憑證設定檔通常會結合其他設定檔類型 (例如 Wi-Fi、VPN 和電子郵件) 使用，以允許使用者驗證公司資源。 當這些設定檔類型與用戶端憑證連結時，設定檔會依賴於該設定檔的成功部署。

初始基礎結構設定和用戶端憑證設定檔相關聯的設定通常需要疑難排解。 如需成功設定 NDES 連接器的逐步指南，以及找出與憑證部署相關問題的疑難排解指導方針，請參閱： 

- [設定基礎結構以使用 Intune 支援 SCEP](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [針對 SCEP 憑證設定檔搭配 Microsoft Intune 進行疑難排解的概觀](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

使用參考的 PowerShell 指令碼來協助驗證您的設定。 如需詳細資訊，請參閱 [Intune 憑證連接器驗證指令碼](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)。

  
**其他常見問題**

**嘗試在 NDES 連接器伺服器上安裝 Intune 憑證連接器時，收到訊息：「無法驗證憑證要求中的密碼。它可能已經被使用。請取得新的密碼，與此要求一起提交。」**  

此訊息表示您必須以系統管理員身分執行憑證連接器安裝。

在某些環境中，Intune 憑證執行所在的伺服器必須使用 Proxy 伺服器來連線到 Intune，因此憑證連接器必須使用 Proxy。 在某些情況下，NDES 連接器會忽略設定的 Proxy 設定，而且在 LocalSystem 的安全性環境中執行時，可能需要設定 Proxy 設定。 
 
解決方案是以 SYSTEM 身分執行 Internet Explorer，並在 IE 中設定 Proxy。 將 Intune 連接器服務重新啟動之後，NDES 連接器就會連線到 Intune。

**使用者裝置不再會從 NDES 接收 SCEP 憑證。**

核發給 NDES 伺服器並在 NDES 連接器安裝期間指定的用戶端驗證憑證，可能已過期或遺失。 若要解決下列問題： 
 
1. 解除安裝 NDES 連接器。  
2. 使用這些詳細資料來要求新的用戶端驗證或伺服器驗證憑證： 
 
    - 主體名稱：CN=外部 FQDN  
    - 主體別名 (兩者都是必要)：DNS=外部 FQDN，DNS=內部 FQDN 
 
3. 使用新的憑證重新安裝 NDES 連接器。