---
title: 升級至 macOS 11.6 Big Sur 之後無法新增帳戶
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475125"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>升級至 macOS 11.6 Big Sur 之後無法新增帳戶

升級至 macOS 11.6 之後，您的公司或學校用 OneDrive 帳戶或 OneDrive 個人帳戶可能不會出現在您的帳戶清單中，而且您可能無法從應用程式登入第二個帳戶。

已針對此問題開發修正程式。 首先，判斷您執行的 OneDrive 是獨立版還是 App Store 版本：

- 選取功能表列中的 OneDrive 雲端 > **[說明與設定]** > **[喜好設定]** > **[關於]**。 如果版本號碼不包含 **(獨立)**，表示您擁有 App Store 版本的產品。

如果您使用獨立版本的 OneDrive，請重新開啟電腦，OneDrive 會自動更新至此問題已解決的組建。 如果您想要手動安裝組建，請下載此 [.zip 檔案](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)、解壓縮該檔案，然後複製 OneDrive 應用程式至 [應用程式資料夾](透過取代現有的 OneDrive 應用程式)。

如果您使用的是 App Store 版本，請考慮安裝獨立版本的 OneDrive。 這個版本與 App Store 版本運作方式相同，但可讓 Microsoft 更快速地為使用者提供更新，並且將它們連接到包含此問題修正程式的版本。

1. 下載 [包含修正程式的 OneDrive](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip) 獨立版本。
2. 解壓縮該檔案，然後複製 OneDrive 應用程式至 [應用程式資料夾](透過取代現有的 OneDrive 應用程式)。

如果您需要使用 App Store 版本，請等待 App Store 發行包含修正程式的應用程式版本。 很抱歉，Microsoft 無法傳達從 App Store 發行固定版本的預估日期。


