---
title: 將 Microsoft Edge 部署到 iOS、iPadOS 和 Android
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8241"
- "9004604"
ms.openlocfilehash: 524e87ab57e29823361053093708c83831f19687
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177993"
---
# <a name="deploy-microsoft-edge-to-ios-ipados-and-android"></a><span data-ttu-id="a1a82-102">將 Microsoft Edge 部署到 iOS、iPadOS 和 Android</span><span class="sxs-lookup"><span data-stu-id="a1a82-102">Deploy Microsoft Edge to iOS, iPadOS, and Android</span></span>

<span data-ttu-id="a1a82-103">下列的指引案例可協助您將 Microsoft Edge 指派給 iOS、iPadOS 和 Android 裝置的使用者。</span><span class="sxs-lookup"><span data-stu-id="a1a82-103">The guided scenario summarized below will help you assign Microsoft Edge to users of iOS, iPadOS, and Android devices.</span></span>

> [!NOTE]
> <span data-ttu-id="a1a82-104">如果您封鎖使用者註冊行動裝置，此指引案例將無法運作，且使用者必須自行安裝 Microsoft Edge。</span><span class="sxs-lookup"><span data-stu-id="a1a82-104">If you blocked users from enrolling mobile devices, this guided scenario won't work and the users will need to install Microsoft Edge on their own.</span></span>

<span data-ttu-id="a1a82-105">指引案例包含下列步驟：</span><span class="sxs-lookup"><span data-stu-id="a1a82-105">The guided scenario involves the following steps:</span></span>

1. [<span data-ttu-id="a1a82-106">先決條件</span><span class="sxs-lookup"><span data-stu-id="a1a82-106">Prerequisites</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#prerequisites)
2. [<span data-ttu-id="a1a82-107">簡介</span><span class="sxs-lookup"><span data-stu-id="a1a82-107">Introduction</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-1---introduction)
3. [<span data-ttu-id="a1a82-108">基本概念</span><span class="sxs-lookup"><span data-stu-id="a1a82-108">Basics</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-2---basics)
4. [<span data-ttu-id="a1a82-109">設定</span><span class="sxs-lookup"><span data-stu-id="a1a82-109">Configuration</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-3---configuration)
5. [<span data-ttu-id="a1a82-110">作業</span><span class="sxs-lookup"><span data-stu-id="a1a82-110">Assignments</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-4---assignments)
6. [<span data-ttu-id="a1a82-111">審閱和建立</span><span class="sxs-lookup"><span data-stu-id="a1a82-111">Review and creation</span></span>](https://docs.microsoft.com/mem/intune/fundamentals/guided-scenarios-edge#step-5---review--create)

<span data-ttu-id="a1a82-112">完成指引案例中的步驟之後，Microsoft Intune 原則將會啟用商務用 Microsoft Edge 的下列功能：</span><span class="sxs-lookup"><span data-stu-id="a1a82-112">After you complete the steps in the guided scenario, Microsoft Intune policies will enable the following features of Microsoft Edge for business:</span></span>

- <span data-ttu-id="a1a82-113">雙重識別</span><span class="sxs-lookup"><span data-stu-id="a1a82-113">Dual identity</span></span>
- <span data-ttu-id="a1a82-114">與 Microsoft Intune 應用程式防護原則相整合</span><span class="sxs-lookup"><span data-stu-id="a1a82-114">Integration with Microsoft Intune app protection policy</span></span>
- <span data-ttu-id="a1a82-115">與 Azure Active Directory 應用程式 Proxy 相整合</span><span class="sxs-lookup"><span data-stu-id="a1a82-115">Integration with Azure Active Directory Application Proxy</span></span>
- <span data-ttu-id="a1a82-116">受管理的 [我的最愛] 和 [首頁] 快速鍵</span><span class="sxs-lookup"><span data-stu-id="a1a82-116">Managed favorites and home page shortcuts</span></span>
