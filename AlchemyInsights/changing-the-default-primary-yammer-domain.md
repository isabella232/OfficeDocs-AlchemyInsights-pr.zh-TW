---
title: 變更預設的 Yammer 網域
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991098"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>變更預設/主要 Yammer 網域

Yammer URL 會包含您 Yammer 網路目前的主要網域名稱。 此網域名稱可能與 Office 365 或 Azure AD 中設定的主要網域名稱不相符。 新增至租用戶的自訂網域數量，以及 Yammer 是否處於受支援的組態 (1 個租用戶：1 個網路，或 1:1)，都會使行為有所差異。 您可以取得有關 [Yammer 網域和 Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) 的文件。

存在多個 Yammer 網路且需要合併，是您看到錯誤網域最常見的原因。 使用網路移轉工具[將資料向下整合到單一網路](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks)是重要的第一步驟。 請先完成此程序，然後再嘗試設定您的主要網域。

**無自訂網域**

針對新的租用戶，Yammer 將會使用該租用戶的預設網域 (例如 fabrikam.onmicrosoft.com)。 主要網域會設為 yammer.com/fabrikam.onmicrosoft.com。

**單一自訂網域**

Yammer 會自動選取租用戶的自訂網域 (例如 fabrikam.com) 作為 Yammer 中的主要網域。 該網域會設定為 yammer.com/fabrikam.com。 這項變更是由網域同步服務所處理，最多可能需要 24 小時才會生效。

**多個自訂網域**

Yammer 可以擁有與預設租用戶網域不同的主要網域。 由於有多個自訂網域，Yammer 不會嘗試從可用網域中猜測正確網域。 您需要開啟支援案例，要求將主要網域名稱變更為您選擇的主要網域。

**其他疑難排解資訊**

在某些情況下，可能因為網域已在租用戶之間移動，因此網域同步服務無法順利執行。 除了不正確的主要網域以外，您可能也會遇到登入或其他問題。 若要解決此問題，您可能需要透過 Microsoft 支援服務將網域移至正確的網路。 這種情況需要直接的協助，且可能需要一些時間來解決，特別是當您有很長的網域名稱清單時。 開啟支援案例，以取得解決這類問題的協助。

當您與支援專員合作時，他們會在您的控管下，檢查網域是否已在租用戶中經過驗證。 如果新增到您租用戶的網域未經過 DNS 的驗證，他們可能會詢問關於您網域的其他驗證問題。 請確認網域已經過 DNS 的驗證，以加快處理速度。
