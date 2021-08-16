---
title: Intune Wi-Fi 設定檔
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
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028211"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi 設定檔

MDM 用戶端的 Wi-Fi 連線成功實作，取決於可反映企業 Wi-Fi 基礎結構需求的正確部署設定檔。 若要檢閱您正在調查的用戶端平台的適當設定，請參閱： 

[在 Microsoft Intune 中為執行 Android 的裝置設定新增 Wi-Fi 設定](https://docs.microsoft.com/intune/wi-fi-settings-android)

[在 Microsoft Intune 中針對 Android Enterprise 專用與完全受控裝置新增 Wi-Fi 設定](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[在 Microsoft Intune 中新增適用於 iOS 與 iPadOS 裝置的 Wi-Fi 設定](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[在 Intune 中為 Windows 10 和更新版本裝置新增 Wi-Fi 設定](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[在 Intune 中為 Windows 裝置匯入 Wi-Fi 設定](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**常見問題**

**我要部署依賴於 Wi-Fi 設定檔中所指定的部署憑證的 Wi-Fi 設定檔。不過，組態設定檔顯示錯誤狀態。**

確定您的裝置已收到憑證。

1. 在 Intune 中，移至 [所有裝置]，然後選取裝置 > [裝置設定]。

2. 確定所有預期的設定檔都已列出，並處於成功狀態。

3. 若是 Android 設定檔，如果您的憑證鏈結中有中繼憑證，請確認已將憑證部署到 Android 裝置。

    若要檢查憑證狀態，請移至 [裝置設定]  >  [設定檔]  >  [Android 中繼 CA]  >  [屬性]  >  [信任的憑證]。

如果您持續看到錯誤，請檢閱程序和疑難排解小節。 如需詳細資訊，請參閱[針對 SCEP 憑證設定檔搭配 Microsoft Intune 進行疑難排解的概觀](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)。

**我將 Wi-Fi 設定檔部署到裝置上。Intune 顯示它已成功完成，但裝置未連線至 Wi-Fi。**

成功狀態表示 Intune 已按照設定成功部署設定檔。 不過，這些設定可能不符合您的網路和/或驗證需求。 如需有關所嘗試連線的詳細資訊，請檢閱基礎結構和驗證服務 (Wi-Fi 存取點控制器和 NPS/RADIUS 伺服器) 中的記錄。 您可能需要與您的網路基礎結構小組或第三方 Wi-Fi 廠商合作，來收集和檢閱記錄。