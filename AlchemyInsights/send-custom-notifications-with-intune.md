---
title: 傳送使用 Intune 自訂通知
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 969649084a2ac536ee1b41f225c3be5415a27c4b
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/27/2019
ms.locfileid: "40886848"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="1004c-102">如何將自訂的通知傳送給受管理的 iOS 和 Android 裝置的使用者</span><span class="sxs-lookup"><span data-stu-id="1004c-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="1004c-103">自訂通知 Intune 處理方式是在使用者的裝置上的公司入口網站應用程式。</span><span class="sxs-lookup"><span data-stu-id="1004c-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="1004c-104">然後，應用程式會建立推播通知該裝置上。</span><span class="sxs-lookup"><span data-stu-id="1004c-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="1004c-105">以下是支援的自訂通知，並再建立 [推入通知的應用程式的回條裝置先決條件：</span><span class="sxs-lookup"><span data-stu-id="1004c-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="1004c-106">裝置必須已安裝的公司入口網站應用程式。</span><span class="sxs-lookup"><span data-stu-id="1004c-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="1004c-107">裝置必須允許傳送推入通知的公司入口網站應用程式。</span><span class="sxs-lookup"><span data-stu-id="1004c-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="1004c-108">當應用程式安裝或更新時，它會提示使用者允許通知。</span><span class="sxs-lookup"><span data-stu-id="1004c-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="1004c-109">Android 裝置必須安裝的 Google 播放服務。</span><span class="sxs-lookup"><span data-stu-id="1004c-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="1004c-110">裝置必須使用 Intune 註冊。</span><span class="sxs-lookup"><span data-stu-id="1004c-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="1004c-111">如需詳細資訊，包括如何傳送一則訊息，請參閱[功能文件](https://docs.microsoft.com/intune/custom-notifications)。</span><span class="sxs-lookup"><span data-stu-id="1004c-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
