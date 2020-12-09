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
ms.openlocfilehash: 2a20f258cbcbca7c8db4e38c52464fefb1b6f39d
ms.sourcegitcommit: 38c87ed786dda7181562492d5d2e7ef0e18e0cab
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/08/2020
ms.locfileid: "49600094"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a><span data-ttu-id="6062f-102">將 Google Chrome extensions 的埠 Chromium 至 Microsoft Edge () </span><span class="sxs-lookup"><span data-stu-id="6062f-102">Port Google Chrome extensions to Microsoft Edge (Chromium)</span></span>

<span data-ttu-id="6062f-103">可輕鬆將 [Google Chrome 擴充功能埠 Chromium 至 Microsoft Edge () ](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)。</span><span class="sxs-lookup"><span data-stu-id="6062f-103">It's easy to [port Google Chrome extensions to Microsoft Edge (Chromium)](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension).</span></span> <span data-ttu-id="6062f-104">在大多數情況下，只需要最小的變更，即可在 Microsoft Edge 上執行這些擴充。</span><span class="sxs-lookup"><span data-stu-id="6062f-104">In most cases, only minimal changes are needed to run these extensions on Microsoft Edge.</span></span>

<span data-ttu-id="6062f-105">Google Chrome 支援的分機 APIs 和資訊清單機碼與 Microsoft Edge 相容。</span><span class="sxs-lookup"><span data-stu-id="6062f-105">The extension APIs and manifest keys supported by Google Chrome are code-compatible with Microsoft Edge.</span></span> <span data-ttu-id="6062f-106">不過，Microsoft Edge 不支援 APIs chrome，getAccounts，chrome，getAuthToken，and chrome. instanceID 的副檔名。</span><span class="sxs-lookup"><span data-stu-id="6062f-106">However, Microsoft Edge does not support the extension APIs chrome.gcm, chrome.identity.getAccounts, chrome.identity.getAuthToken, and chrome.instanceID.</span></span>