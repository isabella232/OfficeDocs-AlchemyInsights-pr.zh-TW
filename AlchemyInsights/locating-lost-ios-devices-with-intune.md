---
title: 使用 Intune 查找遺失的 iOS 裝置
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
- "1283"
- "6700008"
ms.openlocfilehash: af747a63caf76e7b4a4a180eaef25dfdf2cb5e3391079c713fe0e413198efb15
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042297"
---
# <a name="locating-lost-ios-devices-with-intune"></a>使用 Intune 查找遺失的 iOS 裝置

在 iOS 裝置上啟用遺失模式，可讓系統管理員在鎖屏上顯示訊息和連絡人電話號碼。

遺失模式啟用後，系統管理員可使用 [定位裝置] 動作來識別裝置的物理位置。

Intune 中的 [定位裝置] 動作可與 iOS 裝置搭配使用，以在地圖上顯示特定裝置的位置。

若要使用此動作，您的 iOS 裝置必須處於：

- 監督模式
- 遺失模式

如需詳細資訊，請參閱[使用 Intune在 iOS/iPadOS 裝置上啟用遺失模式](https://docs.microsoft.com/intune/device-lost-mode) 以及 [使用 Intune 尋找遺失或失竊的 iOS/iPadOS 裝置](https://docs.microsoft.com/intune/device-locate)。

**常見問題集**

問：我已發布遠端動作來移除裝置上的公司資料，現在它停滯在擱置中的狀態。

答：為了讓遠端動作順利完成，目標裝置必須連上網路且狀況良好。 在下列情況中，遠端動作會停留在擱置狀態達30天，或直到裝置確認該命令為止：

- 當裝置離線。
- 當裝置因 Intune 喪失其管理狀態。

如果您認為裝置已停止簽入，且無法移除公司資料，請選取 [刪除]。 [刪除] 會移除裝置記錄，所以它不會再出現在 Intune 裝置清單中。 如果裝置再次啟動，使用者將必須重新註冊。

問：為什麼我無法使用某些遠端動作？

答：並非所有平臺都支援所有的遠端裝置動作。 下列遠端動作屬於平台特定，因此僅適用于指定的平台。

- 略過啟用鎖定（僅限 iOS）
- 新開始（僅限 Windows）
- 遺失模式（僅限 iOS）
- 定位裝置（僅限 iOS）
- 重新啟動 (僅限 Windows)

如需每個動作的詳細資訊，請參閱 [可用的裝置動作](https://docs.microsoft.com/intune/device-management#available-device-actions)。