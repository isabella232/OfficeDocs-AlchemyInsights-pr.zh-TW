---
title: 疑難排解欺詐偵測檢查的安全性秘訣
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: ab7bd3ec66640d66e5f1ea7c1eeee0a1a9510241
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353240"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>疑難排解欺詐偵測檢查的安全性秘訣

如果您收到的安全提示指出「寄件者未通過欺詐偵測檢查, 而且可能不是誰似乎是」, 則寄件者無法傳遞 DKIM 或 SPF 驗證檢查。 解決此問題的最佳方法是讓寄件者對自己進行授權。 如果寄件者代表您傳送, 您必須將寄件者的 IP 位址新增至您的 SPF 記錄, 以授權使用者。
  
請參閱[疑難排解欺詐偵測的紅色 (可疑) 安全提示](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/), 以取得詳細資訊。
  
以下是一些可協助的連結:
  
- [Office 365 如何使用寄件者原則架構 (SPF) 來防止詐騙](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [在 Office 365 中設定 SPF 以協助防止詐騙](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
