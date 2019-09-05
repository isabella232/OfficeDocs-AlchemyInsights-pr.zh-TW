---
title: 從 SharePoint Online 字詞庫中遺失的字詞
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762043"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>使用 Intune 啟用 Bitlocker 加密

Intune 端點保護原則可以用來設定 Windows 裝置 Boitlocker 加密設定中所述： Windows10 （及更新版本） 來保護裝置使用 Intune 設定

您應該注意執行 Windows 10 的許多較新裝置支援便 MDM 原則的應用程式不會觸發自動 bitlocker 加密。 如果非預設設定，這可能會影響應用程式的原則。 如需詳細資訊，請參閱常見問題集。


常見問題集 問： 哪個版本的 Windows 支援裝置加密使用端點保護原則？
 答： 使用 Bitlocker CSP 實作在 [Intune 端點保護原則設定。並非所有版本，也不版的 Windows 都支援 Bitlocker CSP。 
      在此時間 Windows 版本： 企業;教育版、 行動電話、 行動企業和 Professional （從組建 1809年以前的版本） 支援。




問： 如果裝置已加密使用 Bitlocker 加密方法使用 OS 預設設定，且密碼強度 (XTS-aes-128) 將會套用不同的原則設定會自動觸發重新加密磁碟機使用新的設定嗎？

答：否。 若要套用新的加密設定的磁碟機必須先解密。

附註對於裝置註冊透過 Autopilot 會自動加密，就會發生期間 OOBE 不會觸發直到評估 Intune 原則可讓原則以設定，使用來取代 OS 預設值




問： 如果裝置加密由於 Intune 原則的應用程式將其解密中移除該原則時嗎？

答： 移除加密的相關原則不會導致解密設定的磁碟機。




問： 為什麼 intune 合規性政策顯示我的裝置不一定 「 啟用 Bitlocker 」，但它是？

答: 「 Bitlocker 啟用 「 在 intune 合規性政策設定使用 Windows 裝置健全狀況證明 (DHA) 用戶端。 此用戶端只會在開機時測量裝置狀態。 讓 bitlocker 加密已完成。 如果裝置有已重新開機自 DHA 用戶端服務不會報告為作用中的 bitlocker。