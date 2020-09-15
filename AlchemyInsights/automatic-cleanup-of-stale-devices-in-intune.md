---
title: 自動清除 Intune 中的過時裝置
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
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715012"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>自動清除 Intune 中的過時裝置

Intune 允許管理員設定 90 到 270 天之間的時間間隔，在這之後，將從服務中删除過時裝置。 此設定適用全組織并會立即生效。 任何在超過設定的時間段內未簽入 Intune 服務器的裝置都將被永久删除。

**附註** 只有 MDM 裝置物件符合此清理動作的資格。 排除僅 EAS 裝置物件。

有關裝置何時符合刪除條件基於裝置的清理設定及其「狀態」的詳細資訊:

設定：**在上次簽入日期之後刪除裝置：是 (指定天數 (N) 值)**

- 根據設定中設定的值 (N)，Intune 服務會在上次成功簽入后的指定天數內刪除該裝置。

設定：**刪除上次簽入日期之後的裝置：否**

- 在裝置憑證過期且未續約 180 天之後，裝置就會被刪除。

**注意**，在這兩種情況下，裝置都必須成功在 Intune 上註冊。 在第一次使用 Intune 服務的簽入裝置時註冊。

如果裝置成功註冊到 Intune，但未變成已註冊 Intune 裝置，則會在註冊後的 270 天內刪除該裝置。 (90 天將裝置標示為 [已撤銷]，然後下一個180 天刪除記錄)。

Intune 主控台當前不存在為任何指定裝置建立裝置認證有效期限的機制。 