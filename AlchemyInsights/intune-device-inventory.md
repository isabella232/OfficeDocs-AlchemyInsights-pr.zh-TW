---
title: Intune 裝置庫存
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667869"
---
# <a name="intune-device-inventory"></a>Intune 裝置庫存

設備刀鋒在 Intune 管理中，為每個設備提供管理員深入解析。 顯示的資訊包括：硬體、發現的應用程式、裝置合規性狀態和裝置設定狀態。

硬體和發現的應用程式的庫存資料以每七天為週期收集。 所報告的硬體的應用程式和特定元素因設備作業系統以及設備是個人所有還是公司所有而有所不同。

如需詳細資訊，請參閱[在 Intune 中查看裝置詳細資料](https://docs.microsoft.com/intune/device-inventory)。

**常見問題集**

問：我沒有收到 Intune 註冊的 Windows 裝置上的應用程式完整庫存清單。 為什麼？

答：目前新式應用程式只被列在識別為企業裝置的 Windows 10 PC 上。 Intune 不收集安裝在這些裝置上的 Win32 應用程式相關資訊。

Q：為什麼不從所有裝置收集電話號碼？

A：例如，當執行行動裝置庫存報告時，Intune 中被歸類為企業設備的電話不會被識別為完整的電話號碼。 自帶裝置電話號碼總是用星號（****）部分遮罩，並且只顯示最後四位數。