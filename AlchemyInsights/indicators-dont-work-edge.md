---
title: 使用 Edge 瀏覽器時，指示器無法運作
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651490"
---
# <a name="indicators-dont-work-using-edge-browser"></a>使用 Edge 瀏覽器時，指示器無法運作

建立指示器之後，Edge (Smartscreen) 不使用該指示器。 如需詳細資訊，請參閱[為 IP 和 URL/網域建立指示器](/microsoft-365/security/defender-endpoint/indicator-ip-domain) (部分機器翻譯)。

## <a name="step-1-ensure-the-following"></a>步驟 1：確定下列項目

- 確定指示器正確 (IP/URL 沒有錯字、動作正確、RBAC 群組正確)。
- 建立指示器後至少等待 2 小時，以考慮到任何可能的延遲。
- 確認系統已上線至適用於端點的 Microsoft Defender。
- 確認系統可與雲端通訊。
- 請至[測試網站](https://demo.smartscreen.msft.net)頁面，確認 Smartscreen 已啟用並可連線。

## <a name="step-2-troubleshoot-the-potential-issue"></a>步驟 2：疑難排解可能的問題

- 確定用戶端符合需求。 如需詳細資料，請參閱[為 IP 和 URL/網域建立指示器](/microsoft-365/security/defender-endpoint/indicator-ip-domain) (部分機器翻譯)。
- 確定您執行的是最新版的 Edge 瀏覽器。 若要了解最新版本，請參閱[了解您所擁有的 Microsoft Edge 版本](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)。
- 重新啟動 Edge 瀏覽器。
- 瀏覽至已設定指示器的網站。 如果網站未如預期顯示，請繼續執行步驟 3。 

## <a name="step-3-collect-data"></a>步驟 3：收集資料

- 收集 **MDEClientAnalyzer** 診斷資料。 如需指示，請參閱[將電腦上線至適用於端點的 Microsoft Defender 的問題](issues-with-onboarding-machines.md)。
- 如果您願意安裝及收集 Fiddler 追蹤，請參閱 [Telerik Fiddler](http://www.telerik.com/fiddler)。
- 如果您想獲得 Microsoft 支援服務的指引，請選取下方的 [支援] 圖示以開啟支援案例。
