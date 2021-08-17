---
title: 疑難排解電子文件探索保留錯誤
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1ce8443549ea111bc3ebba9c30c4e621a04926231c24d34c64b6d024194d5249
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886246"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>疑難排解電子文件探索保留錯誤

發生電子文件探索保留問題嗎？ 以下是可考慮的一些最佳做法：

- 檢查保留發佈狀態。  若狀態為 **開啟 (擱置中)** 或 **關閉 (擱置中)**，請等候保留發布完成。
- 將電子文件探索保留更新合併入單一大量要求，而非重複地為每次交易更新此原則。
- 在安全性和合規性中心 PowerShell 中執行 Set-CaseHoldPolicy <policyname> -RetryDistribution。 如需詳細資料，請參閱 [連線到安全性和合規性中心 PowerShel](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell)。

如需緩解及解決電子文件探索保留問題的檢查設定和其它最佳做法的步驟，請參閱 [疑難排解電子文件探索保留錯誤](https://docs.microsoft.com/microsoft-365/compliance/hold-distribution-errors)。
如需有關疑難排解其它常見電子文件探索問題的資訊，請參閱 [調查、疑難排解和解決常見電子文件探索問題](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)。
