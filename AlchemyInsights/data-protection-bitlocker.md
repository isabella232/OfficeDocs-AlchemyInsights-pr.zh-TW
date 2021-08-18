---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: 3f6e48b9d2f7562d74d60c2901759a7ab359e5c67bd4aa2d556d941a41ab680c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54118565"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 啟用 Bitlocker 加密

Intune Endpoint Protection 原則可用於設定 Windows 裝置的 Bitlocker 加密設定。 如需詳細資訊，請參閱[Windows 10 (和更新版本) 設定以使用 Intune 保護裝置](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。

除了 Endpoint Protection 原則之外，也有一個加密報告，可提供裝置之加密狀態的更詳細的視圖。 您可以從 [**裝置 > 監視器**] 底下的 MEM 入口網站存取此報告，然後在 [**設定選取**[加密報告](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/DevicesMonitorMenu/encryptionReport)] 底下存取。

如果您發現 Bitlocker 無法如期啟用，或是用來啟用 Bitlocker 的設定檔處於錯誤狀態，請複查加密報告，以更深入瞭解行為的原因。

若要尋找有關如何轉譯報告（包括各種加密狀態值）的詳細資訊，請參閱 [使用 Intune 監控裝置加密](https://docs.microsoft.com/mem/intune/protect/encryption-monitor)。

您應注意，許多執行 Windows 10 的更新裝置都支援自動 Bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。 如果已設定非預設設定，這可能會影響原則的應用程式。 如需詳細資訊，請參閱下列 FAQ。

如需有關 bitlocker 問題疑難排解的詳細資訊，請參閱[BitLocker Microsoft Intune 中的原則疑難排解](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。
 
 
**常見問題集**

問：哪些版本的 Windows 支援使用 Endpoint Protection 原則的裝置加密？<br>
A： Intune Endpoint Protection 原則中的設定是使用[Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)來執行。 並非所有的版本 Windows 或內部版本都支援 Bitlocker CSP。 <br><br>

問：如何在裝置上啟用 Bitlocker，而不需要使用者進行互動？<br>
A：只要符合必要先決條件，即可透過 Intune 啟用 Bitlocker 「無訊息的加密」。 請參閱裝置需求的詳細資料和範例原則設定，以啟用下列檔中的無訊息加密：以無訊息方式 [啟用 Bitlocker 加密](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)。 <br><br>

Q：如果裝置已使用 Bitlocker 加密方法和密碼長度) AES-128 (預設值的 OS 預設設定來加密，將會以新的設定套用具有不同設定的原則，以自動對該磁片磁碟機重新加密。<br>
答：不能。 若要套用新的密碼設定，必須先解密磁片磁碟機。<br><br>
**附注：** 針對使用 Autopilot 註冊的裝置，在進行 OOBE 原則評估之前，不會觸發在 OOBE 期間進行的自動加密，這可讓您使用原則設定來取代 OS 預設值。
 
Q：如果設備因 Intune 原則的應用而加密，將會在移除該原則時進行解密？<br>
A：移除加密相關原則不會導致解密已設定的磁片磁碟機。
 
問：為什麼 Intune 符合性原則會顯示我的裝置沒有啟用 Bitlocker，即使是？<br>
A： Intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明 (DHA) 用戶端。 此用戶端只會在啟動時測量裝置狀態。 因此，如果在 Bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 Bitlocker 報告為作用中。
 
 