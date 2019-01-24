---
title: 疑難排解詐騙的偵測 safety 秘訣檢查
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29460577"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="eeb17-102">疑難排解詐騙的偵測 safety 秘訣檢查</span><span class="sxs-lookup"><span data-stu-id="eeb17-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="eeb17-p101">如果您是快速 safety 提示會指出"寄件者無法我們詐騙的偵測檢查 and 可能不是誰出現設為"，然後寄件者無法傳遞 DKIM 或 SPF 驗證檢查。若要解決此問題的最佳方法是授權自行寄件者。如果寄件者會將傳送代替您撥打電話，您需要將寄件者的 IP 位址新增至 SPF 記錄授權它們。</span><span class="sxs-lookup"><span data-stu-id="eeb17-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="eeb17-106">如需詳細資訊，請參閱[疑難排解詐騙的偵測紅色 （可疑） safety 秘訣檢查](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/)。</span><span class="sxs-lookup"><span data-stu-id="eeb17-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="eeb17-107">以下是一些可協助的連結：</span><span class="sxs-lookup"><span data-stu-id="eeb17-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="eeb17-108">Office 365 可防止詐騙所使用的寄件者原則架構 (SPF)</span><span class="sxs-lookup"><span data-stu-id="eeb17-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="eeb17-109">在 Office 365 中設定 SPF 以協助防止詐騙</span><span class="sxs-lookup"><span data-stu-id="eeb17-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

