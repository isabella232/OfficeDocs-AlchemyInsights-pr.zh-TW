---
title: 疑難排解欺詐偵測檢查的安全提示
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: c7ee1fcc887a3221b5f2acda1aa6ae6beb03cb96686d4ecb7828a02f8ff48302
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955957"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a>疑難排解欺詐偵測檢查的安全提示

如果您收到的安全提示說「寄件者未通過其欺詐偵測檢查，而且可能不是其似乎是」，表示寄件者無法傳遞 DKIM 或 SPF 驗證檢查。 解決此問題的最佳方法是讓寄件者自行授權。 如果寄件者是代表您傳送，您必須將寄件者的 IP 位址新增至您的 SPF 記錄，以授權這些寄件者。
  
請參閱[疑難排解 red (可疑) 安全提示欺詐偵測檢查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)以取得詳細資訊。
  
以下是一些可協助的連結：
  
- [Microsoft 如何使用寄件者原則框架 (SPF) 以避免欺騙](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [設定 SPF 以協助防止詐騙 ](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
