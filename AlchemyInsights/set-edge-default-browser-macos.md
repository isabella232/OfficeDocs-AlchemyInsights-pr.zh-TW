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
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="fde84-102">在 macOS 裝置上將 Microsoft Edge 設定為預設瀏覽器</span><span class="sxs-lookup"><span data-stu-id="fde84-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="fde84-103">使用這兩個方法之一，將 Microsoft Edge 設定為預設瀏覽器：</span><span class="sxs-lookup"><span data-stu-id="fde84-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="fde84-104">方法 1：使用已將 Microsoft Edge 設定為預設瀏覽器的 macOS 映像為裝置刷機。</span><span class="sxs-lookup"><span data-stu-id="fde84-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="fde84-105">方法 2：設定 DefaultBrowserSettingEnabled 原則，以提示使用者將 Microsoft Edge 設定為預設瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="fde84-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="fde84-106">這兩個方法都會允許使用者變更預設瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="fde84-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="fde84-107">基於此原因，即使您已使用方法 1，也建議您部署 DefaultBrowserSettingEnabled 原則。</span><span class="sxs-lookup"><span data-stu-id="fde84-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="fde84-108">如果使用者在部署原則之後變更預設瀏覽器，該原則會提示使用者將預設瀏覽器設定回 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="fde84-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
