---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731230"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 啟用 Bitlocker 加密

 Intune Endpoint Protection 原則可用於設定 Windows 裝置的 Bitlocker 加密設定。 如需詳細資訊，請參閱 [Windows 10 (和更新版本) 設定，以使用 Intune 保護裝置](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。
 
您應注意，許多執行 Windows 10 的更新裝置都支援自動 Bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。 如果已設定非預設設定，這可能會影響原則的應用程式。 如需詳細資訊，請參閱下列 FAQ。
 
如需有關 bitlocker 問題疑難排解的詳細資訊，請參閱 [疑難排解 Microsoft Intune 中的 BitLocker 原則](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。
 
 
**常見問題集**

 問：哪些版本的 Windows 支援使用 Endpoint Protection 原則裝置加密？<br>
 A： Intune Endpoint Protection 原則中的設定是使用 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)來執行。 並非所有版本或 Windows 組建都支援 Bitlocker CSP。 <br><br>
      目前支援下列 Windows 版本： Enterprise、教育版、行動裝置、行動企業及職業 (組建1809和更新版本) 。
 
Q：如果裝置已使用 Bitlocker 加密方法和密碼長度) AES-128 (預設值的 OS 預設設定來加密，將會以新的設定套用具有不同設定的原則，以自動對該磁片磁碟機重新加密。<br>
答：否。 若要套用新的密碼設定，必須先解密磁片磁碟機。<br><br>
**附注：** 針對使用 Autopilot 註冊的裝置，在進行 OOBE 原則評估之前，不會觸發在 OOBE 期間進行的自動加密，這可讓您使用原則設定來取代 OS 預設值。
 
Q：如果設備因 Intune 原則的應用而加密，將會在移除該原則時進行解密？<br>
A：移除加密相關原則不會導致解密已設定的磁片磁碟機。
 
問：為什麼 Intune 符合性原則會顯示我的裝置沒有啟用 Bitlocker，即使是？<br>
A： Intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明 (DHA) 用戶端。 此用戶端只會在啟動時測量裝置狀態。 因此，如果在 Bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 Bitlocker 報告為作用中。
 
 