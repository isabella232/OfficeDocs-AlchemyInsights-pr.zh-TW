---
title: 透過 Microsoft 365 回覆電子郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: 180bae451941e4aaea94d285362794a797383eca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776477"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a><span data-ttu-id="d2cef-102">設定多功能裝置或應用程式以傳送電子郵件</span><span class="sxs-lookup"><span data-stu-id="d2cef-102">Set up a multifunction device or application to send email</span></span>

<span data-ttu-id="d2cef-103">若要深入了解您的選項和步驟，請參閱[如何將多功能裝置或應用程式設定為使用 Microsoft 365 傳送電子郵件](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365)。</span><span class="sxs-lookup"><span data-stu-id="d2cef-103">To learn about your options and the steps, see [How to set up a multifunction device or application to send email using Microsoft 365](https://docs.microsoft.com/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).</span></span>
  
<span data-ttu-id="d2cef-104">**附註：** 如果您的裝置或應用程式最近已停止運作，請注意我們最近依計劃已開始[停用 3DES 加密](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption)。</span><span class="sxs-lookup"><span data-stu-id="d2cef-104">**Note:** If you have a device or application that recently stopped working, please note we have recently begun [disabling the 3DES cipher](https://docs.microsoft.com/microsoft-365/compliance/technical-reference-details-about-encryption) as planned.</span></span> <span data-ttu-id="d2cef-105">若要查看受影響的裝置，請移至 [SMTP 驗證用戶端報告](https://protection.office.com/mailflow/dashboard)。</span><span class="sxs-lookup"><span data-stu-id="d2cef-105">To see affected devices, go to the [SMTP Auth Clients report](https://protection.office.com/mailflow/dashboard).</span></span> <span data-ttu-id="d2cef-106">常見錯誤可能類似於：身份驗證失敗/錯誤、TLS 失敗/錯誤、密碼演算法錯誤、演算法不相符或連線中斷。</span><span class="sxs-lookup"><span data-stu-id="d2cef-106">Common errors could be similar to: Authentication failure/error, TLS failure/error, Cipher algorithm error, Algorithm mismatch, or Connection dropped.</span></span> <span data-ttu-id="d2cef-107">若要解決此問題：</span><span class="sxs-lookup"><span data-stu-id="d2cef-107">To resolve the issue:</span></span>

 - <span data-ttu-id="d2cef-108">**將無法使用 Windows Server 2003 IIS SMTP – 需要較新版本的 Windows。**</span><span class="sxs-lookup"><span data-stu-id="d2cef-108">**Windows Server 2003 IIS SMTP will no longer work – a newer version of Windows is required.**</span></span>  
 - <span data-ttu-id="d2cef-109">請洽詢您的應用程式或裝置廠商，查看是否支援新式密碼，或者是否提供更新。</span><span class="sxs-lookup"><span data-stu-id="d2cef-109">Please check with your application or device vendor to see if a modern cipher is supported or if there is an update.</span></span>
