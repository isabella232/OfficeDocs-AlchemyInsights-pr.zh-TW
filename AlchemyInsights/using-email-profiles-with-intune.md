---
title: 使用 Intune 電子郵件設定檔
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653279"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="7a8d4-102">使用 Intune 電子郵件設定檔</span><span class="sxs-lookup"><span data-stu-id="7a8d4-102">Using email profiles with Intune</span></span>

<span data-ttu-id="7a8d4-103">您可使用 Intune 在多個裝置平台上建立並部署本機 (內建 ) 電子郵件用戶端的電子郵件設定檔。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="7a8d4-104">關於電子郵件設定檔相關的某些限制的資訊 (包括如何處理現有設定檔的顯示狀態，以及如何移除電子郵件設定檔)，請參閱[使用 Intune 新增電子郵件設定到裝置](https://docs.microsoft.com/intune/email-settings-configure)。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="7a8d4-105">有關如何為每個裝置平台建立電子郵件設定檔的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="7a8d4-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="7a8d4-106">Android 裝置設定在 Intune 中設定電子郵件、驗證和同步</span><span class="sxs-lookup"><span data-stu-id="7a8d4-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="7a8d4-107">iOS 和 iPadOS 裝置在 Microsoft Intune 中新增電子郵件設定</span><span class="sxs-lookup"><span data-stu-id="7a8d4-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="7a8d4-108">執行 Windows Phone 8.1 的裝置在 Microsoft Intune 中的電子郵件設定檔設定。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="7a8d4-109">執行 Windows 10 的裝置在 Microsoft Intune 中的電子郵件設定檔設定</span><span class="sxs-lookup"><span data-stu-id="7a8d4-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="7a8d4-110">**常見的同步問題**</span><span class="sxs-lookup"><span data-stu-id="7a8d4-110">**Common syncing issue**</span></span>

<span data-ttu-id="7a8d4-111">**Android 電子郵件設定檔上的 KNOX 可防止使用者的連絡人、行事曆及工作同步至使用者裝置。**</span><span class="sxs-lookup"><span data-stu-id="7a8d4-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="7a8d4-112">Android KNOX 電子郵件設定檔上的 KNOX 提供管理員通過啟要同步的內容類型來決定要將哪些內容類型同步處理到裝置的選項。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="7a8d4-113">如果任何內容類型的被設定為**未設定** (預設)，該內容類型就不會自動同步。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="7a8d4-114">使用者可以直接在裝置上手動啟用所需的內容類型，但該設定會被 Intune 原則設定所覆寫，並且該內容類型的同步將停止。</span><span class="sxs-lookup"><span data-stu-id="7a8d4-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

