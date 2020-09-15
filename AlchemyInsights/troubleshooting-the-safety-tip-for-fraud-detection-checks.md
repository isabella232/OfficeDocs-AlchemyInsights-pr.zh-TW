---
title: 疑難排解欺詐偵測檢查的安全性秘訣
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658401"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="65b92-102">疑難排解欺詐偵測檢查的安全性秘訣</span><span class="sxs-lookup"><span data-stu-id="65b92-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="65b92-103">如果您取得的安全性提示是「寄件者未通過我們的欺詐偵測檢查，而且可能不是誰似乎是」，表示寄件者無法傳遞 DKIM 或 SPF 驗證檢查。</span><span class="sxs-lookup"><span data-stu-id="65b92-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="65b92-104">解決此問題的最佳方法是讓寄件者自行授權。</span><span class="sxs-lookup"><span data-stu-id="65b92-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="65b92-105">如果寄件者是代表您傳送，您必須將寄件者的 IP 位址新增至您的 SPF 記錄，以授權這些寄件者。</span><span class="sxs-lookup"><span data-stu-id="65b92-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="65b92-106">請參閱 [疑難排解 red (可疑) 安全提示以進行欺詐偵測檢查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) 以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="65b92-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="65b92-107">以下是一些可協助的連結：</span><span class="sxs-lookup"><span data-stu-id="65b92-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="65b92-108">Microsoft 如何使用寄件者原則框架 (SPF) 以避免欺騙</span><span class="sxs-lookup"><span data-stu-id="65b92-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="65b92-109">設定 SPF 以協助防止詐騙</span><span class="sxs-lookup"><span data-stu-id="65b92-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
