---
title: VPN 相關問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970970"
---
# <a name="vpn-related-issues"></a>VPN 相關問題

MDM 用戶端的 VPN 連線成功實作，取決於可反映 VPN 基礎結構需求的正確部署設定檔。 有關正在調查的用戶端平台的適當設定，請參閱： 

[Windows 10 和 Windows 全息攝影版裝置設定使用 Intune 新增 VPN 連線](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[在 Microsoft Intune 中新增適用於 iOS 與 iPadOS 裝置的 VPN 設定](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Android 裝置設定在 Intune 中設定 VPN ](https://docs.microsoft.com/intune/vpn-settings-android)  
[macOS 裝置新增 Microsoft Intune 中的 VPN 設定](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

如果您的 VPN 設定檔使用憑證型驗證，請確認已成功部署連結至 VPN 設定檔的根憑證和用戶端驗證憑證設定檔。

**常見問題**

**我將 VPN 設定檔部署到裝置上。Intune 顯示它已成功完成，但裝置未連線至 VPN。**

成功狀態表示 Intune 已按照設定成功部署設定檔。 不過，這些設定可能不符合您的網路和/或驗證需求。 如需有關所嘗試連線的詳細資訊，請檢閱基礎結構和驗證服務 (VPN 伺服器和 NPS/RADIUS 伺服器) 中的記錄。 您可能需要與您的網路基礎結構小組或第三方 VPN 廠商合作，來收集和檢閱記錄。

**當我設定 iOS 版自訂 VPN 時，無法使用個別應用程式的 VPN 功能。**

iOS 裝置 Intune 中的個別應用程式 VPN 目前可供特定的提供者和合作夥伴使用，這些人在設定個別應用程式 VPN 之前，必須同時符合憑證先決條件。 如需詳細資訊，請參閱[iOS/iPadOS 裝置在 Intune 中設定個別應用程式虛擬私人網路 (VPN)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)。 

如需有關 Intune 中所有 VPN 連線類型的詳細資訊，請參閱[建立 VPN 設定檔以連接到 Intune 中的 VPN 伺服器](https://docs.microsoft.com/intune/vpn-settings-configure)。  

**當存取已設定的網域時，未觸發 iOS 的隨選 VPN**

若要測試自動 VPN 設定，請設定下列值：

我想要執行下列操作： **評估每個連線嘗試** 

選擇是否要連線：**如有需要，請連線**

當使用者存取下列網域時： **目標***網域名稱*

如果上述設定失敗，請新增下列元素：

無法連線此 URL 時，強制連線 VPN：**BADURL**