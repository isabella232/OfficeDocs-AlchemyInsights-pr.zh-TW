---
title: 使用 Intune 傳送自訂通知
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720637"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="c4e94-102">如何將自訂通知傳送給受管理的 iOS 和 Android 裝置的使用者</span><span class="sxs-lookup"><span data-stu-id="c4e94-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="c4e94-103">自訂的 Intune 通知是由使用者裝置上的公司入口網站應用程式處理。</span><span class="sxs-lookup"><span data-stu-id="c4e94-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="c4e94-104">然後，應用程式會在該裝置上建立推播通知。</span><span class="sxs-lookup"><span data-stu-id="c4e94-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="c4e94-105">以下是支援接收自訂通知的裝置必要條件，然後讓應用程式建立推播通知：</span><span class="sxs-lookup"><span data-stu-id="c4e94-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="c4e94-106">裝置必須已安裝公司入口網站應用程式。</span><span class="sxs-lookup"><span data-stu-id="c4e94-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="c4e94-107">裝置必須允許公司入口網站應用程式傳送推播通知。</span><span class="sxs-lookup"><span data-stu-id="c4e94-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="c4e94-108">安裝或更新應用程式時，會提示使用者允許通知。</span><span class="sxs-lookup"><span data-stu-id="c4e94-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="c4e94-109">Android 裝置必須已安裝 Google Play 服務。</span><span class="sxs-lookup"><span data-stu-id="c4e94-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="c4e94-110">裝置必須使用 Intune 註冊。</span><span class="sxs-lookup"><span data-stu-id="c4e94-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="c4e94-111">如需詳細資訊，包括如何傳送郵件，請參閱 [功能檔](https://docs.microsoft.com/intune/custom-notifications)。</span><span class="sxs-lookup"><span data-stu-id="c4e94-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
