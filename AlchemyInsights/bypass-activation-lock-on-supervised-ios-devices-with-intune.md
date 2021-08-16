---
title: 使用 Intune 在監督的 iOS 裝置上略過啟用鎖定
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: de52ba77d3155d957372c31d465881fc7e8fcbbe657dfa35dedfee2be52e5a52
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046491"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>使用 Intune 在監督的 iOS 裝置上略過啟用鎖定

在 iOS 裝置上略過啟用鎖定的功能，可讓您更輕鬆地從使用者啟用公司裝置上的啟用鎖定，然後離開公司。

跳過啟用鎖定的先決條件包括：

- 裝置是「受監督的」。
- 啟用鎖定已在 Intune 中使用 iOS 裝置限制原則成功啟用。

此外，如果略過啟用鎖定，您應：

- 實際擁有資料被擦除的裝置。
- 在您發布擦除命令之前，先複製程式碼。

**注意：** [擦除程式碼] 不區分大小寫，因此不需要 "-" 字元。

如需詳細資訊，請參閱 [以 Intune 在受監督的 iOS 裝置上略過啟用所訂](https://docs.microsoft.com/intune/device-activation-lock-bypass)。

**常見問題集**

問： **我已發布遠端動作來移除裝置上的公司資料，現在它停滯在擱置中的狀態。**

答：為了讓遠端動作順利完成，目標裝置必須連上網路且狀況良好。 在下列情況中，遠端動作會停留在擱置狀態達30天，或直到裝置在以下狀況中確認該命令為止：

- 沒有連線。
- 因 Intune 喪失其管理狀態。

如果您認為裝置已停止簽入，且無法移除公司資料，請選取 [刪除]。 [刪除] 會移除裝置記錄，所以它不會再出現在 Intune 裝置清單中。 若要讓裝置再次啟用，其使用者必須重新註冊裝置。

問： **為什麼我無法使用某些遠端動作？**

答：並非所有平臺都支援所有的遠端裝置動作。 下列遠端動作屬於平臺特定。

- 略過啟用鎖定（僅限 iOS）
- 新開始（僅限 Windows）
- 遺失模式（僅限 iOS）
- 定位裝置（僅限 iOS）
- 重新啟動 (僅限 Windows)

如需每個動作的詳細資訊，請參閱 [可用的裝置動作](https://docs.microsoft.com/intune/device-management#available-device-actions)。