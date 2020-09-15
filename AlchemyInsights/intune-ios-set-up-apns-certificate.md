---
title: Intune iOS 的 APNS 憑證設定
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
- "9000654"
- "3543"
ms.openlocfilehash: f58405de018c916e08672022bb4f66292524b736
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667437"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="a68b9-102">Intune iOS 的 APNS 憑證設定</span><span class="sxs-lookup"><span data-stu-id="a68b9-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="a68b9-103">您的訂閱上尚未設定 Apple MDM 推播憑證 (又稱為 Apple 推播通知服務 (APN) 憑證)。</span><span class="sxs-lookup"><span data-stu-id="a68b9-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="a68b9-104">如果沒有設定 Apple MDM 推播憑證，您將無法註冊及管理 iOS 和 MacOS 裝置。</span><span class="sxs-lookup"><span data-stu-id="a68b9-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="a68b9-105">將憑證新增至 Intune 之後，您的使用者就可以安裝公司入口網站應用程式來註冊其 iOS 裝置。</span><span class="sxs-lookup"><span data-stu-id="a68b9-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="a68b9-106">如需將 APNS 憑證新增到 Intune 租用戶的逐步指南，請查看下列連結的內容：</span><span class="sxs-lookup"><span data-stu-id="a68b9-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="a68b9-107">取得 Apple MDM 推播憑證</span><span class="sxs-lookup"><span data-stu-id="a68b9-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="a68b9-108">如果您遇到 Apple 推播通知憑證 (APN) 的相關問題，請參閱此部落格文章：[Intune 和 APN 憑證：常見問題集](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="a68b9-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
