---
title: '埠 Microsoft Edge (Chromium 的 Google Chrome 擴充功能) '
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
ms.openlocfilehash: 34ec7e71a2f27eb5b46395876a4d1c903189be1050e523796c9f2a817c20aaa0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53973688"
---
# <a name="port-google-chrome-extensions-to-microsoft-edge-chromium"></a>埠 Microsoft Edge (Chromium 的 Google Chrome 擴充功能) 

可輕鬆將[Google Chrome 擴充的埠設為 Microsoft Edge (Chromium) ](https://docs.microsoft.com/microsoft-edge/extensions-chromium/developer-guide/port-chrome-extension)。 在大多數情況下，只需要最少的變更，即可在 Microsoft Edge 上執行這些擴充。

Google Chrome 所支援的分機 APIs 和資訊清單機碼與 Microsoft Edge 的程式碼相容。 不過，Microsoft Edge 不支援副檔名 APIs chrome，getAccounts，chrome，getAuthToken，and chrome. instanceID。