---
title: '將 Google Chrome extensions 的埠 Chromium 至 Microsoft Edge () '
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004032"
- "7102"
- "8297"
- "9004617"
ms.openlocfilehash: 1c71d74d01c1e38e4c7789aea2c0b43701b3a5de
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505275"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="139f2-102">將 Google Chrome extensions 的埠 Chromium 至 Microsoft Edge () </span><span class="sxs-lookup"><span data-stu-id="139f2-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="139f2-103">可輕鬆將 [Google Chrome 擴充功能埠 Chromium 至 Microsoft Edge () ](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)。</span><span class="sxs-lookup"><span data-stu-id="139f2-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="139f2-104">在大多數情況下，只需要最小的變更，即可在 Microsoft Edge 上執行這些擴充。</span><span class="sxs-lookup"><span data-stu-id="139f2-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="139f2-105">Google Chrome 支援的分機 APIs 和資訊清單機碼與 Microsoft Edge 相容。</span><span class="sxs-lookup"><span data-stu-id="139f2-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="139f2-106">不過，Microsoft Edge 不支援 APIs chrome，getAccounts，chrome，getAuthToken，and chrome. instanceID 的副檔名。</span><span class="sxs-lookup"><span data-stu-id="139f2-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>