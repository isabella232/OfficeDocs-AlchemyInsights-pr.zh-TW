---
title: 在 macOS 裝置上將 Microsoft Edge 設定為預設瀏覽器
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: e04f8931ef12c426a5c3d5f617fc5f5d5c3a15c6fe43f7b84a7e97e8ee04e3fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54073951"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>在 macOS 裝置上將 Microsoft Edge 設定為預設瀏覽器

使用這兩個方法之一，將 Microsoft Edge 設定為預設瀏覽器：

方法 1：使用已將 Microsoft Edge 設定為預設瀏覽器的 macOS 映像為裝置刷機。

方法 2：設定 DefaultBrowserSettingEnabled 原則，以提示使用者將 Microsoft Edge 設定為預設瀏覽器。

這兩個方法都會允許使用者變更預設瀏覽器。 基於此原因，即使您已使用方法 1，也建議您部署 DefaultBrowserSettingEnabled 原則。 如果使用者在部署原則之後變更預設瀏覽器，該原則會提示使用者將預設瀏覽器設定回 Microsoft Edge。
