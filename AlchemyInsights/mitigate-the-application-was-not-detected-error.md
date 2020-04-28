---
title: 緩解未偵測到應用程式的錯誤
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: e07c6b128a39f1fb1c998d051aafe72205d8cbee
ms.sourcegitcommit: 82155846ce771c18050e6113d6c199b34a1504ff
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/24/2020
ms.locfileid: "43810475"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="309e1-102">緩解「未偵測到應用程式」的錯誤</span><span class="sxs-lookup"><span data-stu-id="309e1-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="309e1-103">在所有主要的 OS 平台 (Windows、iOS 和 Android) 上，都可能發生由 Intune 回報的應用程式安裝錯誤：「未偵測到成功完成安裝後的應用程式」。</span><span class="sxs-lookup"><span data-stu-id="309e1-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="309e1-104">最常產生此錯誤的情況包括：</span><span class="sxs-lookup"><span data-stu-id="309e1-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="309e1-105">初次部署之後，應用程式在 Intune 外部 (從第三方應用程式商店) 進行更新。</span><span class="sxs-lookup"><span data-stu-id="309e1-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="309e1-106">例如，某些應用程式 (例如 Google Chrome) 可能會執行自動更新。</span><span class="sxs-lookup"><span data-stu-id="309e1-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="309e1-107">初次安裝後，使用者將應用程式解除安裝。</span><span class="sxs-lookup"><span data-stu-id="309e1-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="309e1-108">若要緩解此問題，請先檢查受影響的裝置，以判斷發生錯誤的情形。</span><span class="sxs-lookup"><span data-stu-id="309e1-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="309e1-109">如果應用程式已於 Intune 外部更新，可以將應用程式部署設定為忽略應用程式版本。</span><span class="sxs-lookup"><span data-stu-id="309e1-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="309e1-110">若要這麼做，請在 [應用程式設定] > [應用程式資訊]\*\*\*\* 底下，將 [忽略應用程式版本]\*\*\*\* 設為 [是]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="309e1-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="309e1-111">若以用戶端為目標，建議您將應用程式部署為「必要」，並確定部署的是最新版本。</span><span class="sxs-lookup"><span data-stu-id="309e1-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="309e1-112">或者，在 iOS 平台上，您可以使用與 Apple 大量採購方案 (Volume Purchase Program) 關聯的**自動更新**功能，以設定為在新應用程式版本推出時自動更新。</span><span class="sxs-lookup"><span data-stu-id="309e1-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="309e1-113">如需針對應用程式安裝問題進行疑難排解的詳細資訊，請參閱[針對應用程式安裝問題進行疑難排解](https://docs.microsoft.com/intune/troubleshoot-app-install)。</span><span class="sxs-lookup"><span data-stu-id="309e1-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
