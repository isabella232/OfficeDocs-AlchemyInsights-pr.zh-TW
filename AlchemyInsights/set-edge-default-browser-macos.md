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
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426787"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>在 macOS 裝置上將 Microsoft Edge 設定為預設瀏覽器

使用這兩個方法之一，將 Microsoft Edge 設定為預設瀏覽器：

方法 1：使用已將 Microsoft Edge 設定為預設瀏覽器的 macOS 映像為裝置刷機。

方法 2：設定 DefaultBrowserSettingEnabled 原則，以提示使用者將 Microsoft Edge 設定為預設瀏覽器。

這兩個方法都會允許使用者變更預設瀏覽器。 基於此原因，即使您已使用方法 1，也建議您部署 DefaultBrowserSettingEnabled 原則。 如果使用者在部署原則之後變更預設瀏覽器，該原則會提示使用者將預設瀏覽器設定回 Microsoft Edge。
