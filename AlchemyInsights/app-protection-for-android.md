---
title: Microsoft Intune 中的 Android 應用程式保護原則設定
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/20/2020
ms.locfileid: "49373941"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="9068d-102">Microsoft Intune 中的 Android 應用程式保護原則設定</span><span class="sxs-lookup"><span data-stu-id="9068d-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="9068d-103">Android 裝置的應用程式保護原則設定有三種類別：</span><span class="sxs-lookup"><span data-stu-id="9068d-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="9068d-104">**資料保護** 控制公司資料的處理方式，例如，是否可以複製或貼上資料至不同的應用程式，或是否可以讓應用程式取得螢幕擷取畫面。</span><span class="sxs-lookup"><span data-stu-id="9068d-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="9068d-105">設定也會在公司資料上強制執行加密，並管理特定資料是否可以與原生裝置應用程式同步處理，如連絡人清單或網頁瀏覽器。</span><span class="sxs-lookup"><span data-stu-id="9068d-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="9068d-106">若要深入瞭解，請參閱 [資料保護](https://go.microsoft.com/fwlink/?linkid=2135259)。</span><span class="sxs-lookup"><span data-stu-id="9068d-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="9068d-107">**存取需求** 會指導使用者存取應用程式的方式。</span><span class="sxs-lookup"><span data-stu-id="9068d-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="9068d-108">例如，應用程式可能需要使用者輸入 PIN 或指紋才能存取。</span><span class="sxs-lookup"><span data-stu-id="9068d-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="9068d-109">若要深入瞭解，請參閱 [Access 需求](https://go.microsoft.com/fwlink/?linkid=2135260)。</span><span class="sxs-lookup"><span data-stu-id="9068d-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="9068d-110">**條件式發佈** 會控制應用程式的登入安全性設定，例如，鎖定前的最大 PIN 碼嘗試，或執行應用程式所需的最低作業系統。</span><span class="sxs-lookup"><span data-stu-id="9068d-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="9068d-111">若要深入瞭解，請參閱 [條件式發行](https://go.microsoft.com/fwlink/?linkid=2135507)。</span><span class="sxs-lookup"><span data-stu-id="9068d-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>
