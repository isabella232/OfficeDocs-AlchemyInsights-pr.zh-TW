---
title: SharePoint 線上術語存放區中遺失的字詞
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750442"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 啟用 Bitlocker 加密

您可以使用 intune Endpoint Protection 原則，設定 Windows 裝置的 Boitlocker 加密設定，如中所述： Windows10 (和更新版本) 設定，以使用 Intune 保護裝置

您應注意，許多執行 Windows 10 的更新裝置都支援自動 bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。 如果未設定預設設定，這可能會影響原則的應用程式。 如需詳細資訊，請參閱 FAQ。


FAQ   Q：哪些版本的 Windows 支援使用 Endpoint Protection 原則的裝置加密？
 A： Intune Endpoint Protection 原則中的設定是使用 Bitlocker CSP 來執行。並非所有的版本和 Windows 內部版本都支援 Bitlocker CSP。 
      在此時間，Windows 版本： Enterprise;支援從 build 1809 向上) 所提供的教育版、行動裝置、行動企業版及職業 (。




Q：如果裝置已使用 Bitlocker 加密方法和密碼 (長度的 OS 預設值設定，以 Bitlocker 加密，) 將會以新的設定套用具有不同設定的原則，將會自動對該磁片磁碟機重新加密 XTS-AES-128。

答：否。 為了套用新的密碼設定，必須先解密磁片磁碟機。

附注：針對使用 Autopilot 註冊的裝置，將不會觸發在 OOBE 期間進行的自動加密，除非已評估 Intune 原則，才能使用原則設定來取代 OS 預設值




Q：如果裝置因 Intune 原則的應用而加密，將會在移除該原則時進行解密？

A：移除加密相關原則不會導致解密已設定的磁片磁碟機。




問：為什麼 intune 符合性原則會顯示我的裝置沒有「啟用 Bitlocker」，但它是？

A： intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明 (DHA) 用戶端。 此用戶端只會在啟動時測量裝置狀態。 因此，如果在 bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 bitlocker 報告為作用中。