---
title: 疑難排解詐騙偵測安全提示檢查
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
ms.openlocfilehash: 7ce8bcc7caefebf51fc8d9622367fd16405deef1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533152"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="06885-102">疑難排解詐騙偵測安全提示檢查</span><span class="sxs-lookup"><span data-stu-id="06885-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="06885-103">如果您是取得安全提示會說 「 寄件者失敗我們詐騙偵測檢查的而且可能看起來會是誰，「 再寄件者無法通過 SPF 或 DKIM 驗證檢查。</span><span class="sxs-lookup"><span data-stu-id="06885-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="06885-104">若要解決此問題的最佳方法是寄件者授權本身。</span><span class="sxs-lookup"><span data-stu-id="06885-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="06885-105">如果寄件者代表您傳送，您需要將其授權透過將寄件者的 IP 位址新增至您的 SPF 記錄。</span><span class="sxs-lookup"><span data-stu-id="06885-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="06885-106">如需詳細資訊，請參閱[疑難排解詐騙偵測紅色 （可疑） 的安全提示檢查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。</span><span class="sxs-lookup"><span data-stu-id="06885-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="06885-107">以下是一些可協助的連結：</span><span class="sxs-lookup"><span data-stu-id="06885-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="06885-108">Office 365 如何使用寄件者原則架構 (SPF) 來防範詐騙</span><span class="sxs-lookup"><span data-stu-id="06885-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="06885-109">在 Office 365 中設定 SPF 以協助防止詐騙</span><span class="sxs-lookup"><span data-stu-id="06885-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
