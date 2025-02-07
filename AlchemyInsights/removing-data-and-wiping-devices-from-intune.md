---
title: 從 Intune 中移除資料和抹除裝置
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
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: 92673c4a2a0e0faa98d3ade5ca1f6aa687d4c94a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331032"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>從 Intune 中移除資料和抹除裝置

設備淘汰和設備抹除遠端操作可用於移除 Intune 管理的公司資料，或執行出廠預設並將設備恢復為其默認設置。

1. 登入 Microsoft 365 裝置管理，然後移至 **裝置** > **所有裝置**。
2. 選取您要抹除的裝置。
3. 選取您要執行的遠端抹除類型。 [淘汰] 只會刪除組織資訊，而完整的抹除則會將裝置還原為出廠預設。
4. 選取 **[是]** 加以確認。 裝置動作狀態將顯示為 *停用擱置*，直到抹除完成為止。
    操作完成之後，您將不會再在受管理裝置清單中看到該行動裝置。

**附註**：無法從「已加入」Azure AD 的裝置移除公司資料。 

如需淘汰和抹除動作影響的完整詳細資料 (包括保留內容和刪除內容)，請參閱以下文件:

- [使用抹除、淘汰或手動取消註冊裝置來移除裝置](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)。
- [如何只抹除 Intune 管理之應用程式中的公司資料](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- [清除 macOS 裝置的所有資料](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)。