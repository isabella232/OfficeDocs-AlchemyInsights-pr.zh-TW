---
title: 為行動裝置部署 Microsoft Edge 以供 iOS/iPadOS 或 Android
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
- "9003919"
- "6974"
ms.openlocfilehash: 98ab637b6ca0f2b3cfa98ae897d6ed1d9f36c3cd
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/11/2020
ms.locfileid: "49652140"
---
# <a name="deploy-microsoft-edge-for-mobile-for-iosipados-or-android"></a><span data-ttu-id="f5937-102">為行動裝置部署 Microsoft Edge 以供 iOS/iPadOS 或 Android</span><span class="sxs-lookup"><span data-stu-id="f5937-102">Deploy Microsoft Edge for Mobile for iOS/iPadOS or Android</span></span>

<span data-ttu-id="f5937-103">下列的導向案例會協助您將 Microsoft Edge 指派給 iOS、iPadOS 及 Android 裝置的使用者。</span><span class="sxs-lookup"><span data-stu-id="f5937-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span> <span data-ttu-id="f5937-104">在您完成這些步驟之後，Microsoft Intune 原則將為商務用 Microsoft Edge 啟用下列功能：</span><span class="sxs-lookup"><span data-stu-id="f5937-104">After you complete these steps, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="f5937-105">雙重身分識別</span><span class="sxs-lookup"><span data-stu-id="f5937-105">Dual identity</span></span>
- <span data-ttu-id="f5937-106">與 Microsoft Intune 應用程式保護原則整合</span><span class="sxs-lookup"><span data-stu-id="f5937-106">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="f5937-107">與 Azure Active Directory 應用程式 Proxy 整合</span><span class="sxs-lookup"><span data-stu-id="f5937-107">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="f5937-108">受管理的我的最愛及首頁快捷方式</span><span class="sxs-lookup"><span data-stu-id="f5937-108">Managed favorites and home page shortcuts</span></span>

> [!NOTE]
> <span data-ttu-id="f5937-109">如果您封鎖使用者未註冊行動裝置，此導向案例將無法運作，而且使用者將需要自行安裝 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="f5937-109">If you blocked users from enrolling mobile devices, this guided scenario will not work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="f5937-110">若要為行動裝置部署 iOS/iPadOS 或 Android 的 Microsoft Edge，請參閱：</span><span class="sxs-lookup"><span data-stu-id="f5937-110">To deploy Microsoft Edge for Mobile for iOS/iPadOS or Android, see:</span></span>

1. [<span data-ttu-id="f5937-111">先決條件</span><span class="sxs-lookup"><span data-stu-id="f5937-111">Prerequisites</span></span>](https://go.microsoft.com/fwlink/?linkid=2133027)
2. [<span data-ttu-id="f5937-112">簡介</span><span class="sxs-lookup"><span data-stu-id="f5937-112">Introduction</span></span>](https://go.microsoft.com/fwlink/?linkid=2133520)
3. [<span data-ttu-id="f5937-113">基本概念</span><span class="sxs-lookup"><span data-stu-id="f5937-113">Basics</span></span>](https://go.microsoft.com/fwlink/?linkid=2133421)
4. [<span data-ttu-id="f5937-114">設定</span><span class="sxs-lookup"><span data-stu-id="f5937-114">Configuration</span></span>](https://go.microsoft.com/fwlink/?linkid=2133521)
5. [<span data-ttu-id="f5937-115">指派</span><span class="sxs-lookup"><span data-stu-id="f5937-115">Assignments</span></span>](https://go.microsoft.com/fwlink/?linkid=2132869)
6. [<span data-ttu-id="f5937-116">審閱和建立</span><span class="sxs-lookup"><span data-stu-id="f5937-116">Review and creation</span></span>](https://go.microsoft.com/fwlink/?linkid=2133522)
