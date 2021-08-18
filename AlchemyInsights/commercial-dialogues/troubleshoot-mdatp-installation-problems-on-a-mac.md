---
title: 疑難排解 Mac 上的 MDATP 安裝問題
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090983"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>疑難排解 Mac 上的 MDATP 安裝問題

若手動安裝失敗，安裝精靈的 [ **摘要** ] 頁面會顯示下列錯誤：

「安裝時發生錯誤。 安裝程式發生錯誤，導致安裝失敗。 請與軟體製造商聯繫以取得協助。」

在 MDM 部署中，頁面也會顯示一般安裝失敗。

雖然我們沒有向使用者顯示確切的錯誤，我們還是會在 **/Library/Logs/Microsoft/mdatp/install.log** 中保留具有安裝進度的記錄檔。 每個安裝會話都會附加到此記錄檔。 若只要輸出上一個安裝會話，請使用 `sed` 。

若要深入瞭解，請參閱 [疑難排解 Microsoft DEFENDER ATP For Mac 的安裝問題](https://go.microsoft.com/fwlink/?linkid=2144615)。
