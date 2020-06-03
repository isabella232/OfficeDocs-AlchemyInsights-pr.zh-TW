---
title: 疑難排解欺詐偵測檢查的安全性秘訣
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 74913492a086de688067d588e95dd87e6946743b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44504974"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>疑難排解欺詐偵測檢查的安全性秘訣

如果您取得的安全性提示是「寄件者未通過我們的欺詐偵測檢查，而且可能不是誰似乎是」，表示寄件者無法傳遞 DKIM 或 SPF 驗證檢查。 解決此問題的最佳方法是讓寄件者自行授權。 如果寄件者是代表您傳送，您必須將寄件者的 IP 位址新增至您的 SPF 記錄，以授權這些寄件者。
  
請參閱[疑難排解紅色（可疑）安全性秘訣，以取得欺詐偵測檢查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)的詳細資訊。
  
以下是一些可協助的連結：
  
- [Microsoft 如何使用寄件者原則架構（SPF）來防止欺騙](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [設定 SPF 以協助防止詐騙](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
