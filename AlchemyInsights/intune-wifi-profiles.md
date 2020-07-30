---
title: Intune Wi-Fi 設定檔
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509054"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="ffb8e-102">Intune Wi-Fi 設定檔</span><span class="sxs-lookup"><span data-stu-id="ffb8e-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="ffb8e-103">MDM 用戶端的 Wi-Fi 連線成功實作，取決於可反映企業 Wi-Fi 基礎結構需求的正確部署設定檔。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="ffb8e-104">若要檢閱您正在調查的用戶端平台的適當設定，請參閱：</span><span class="sxs-lookup"><span data-stu-id="ffb8e-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="ffb8e-105">在 Microsoft Intune 中為執行 Android 的裝置設定新增 Wi-Fi 設定</span><span class="sxs-lookup"><span data-stu-id="ffb8e-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="ffb8e-106">在 Microsoft Intune 中針對 Android Enterprise 專用與完全受控裝置新增 Wi-Fi 設定</span><span class="sxs-lookup"><span data-stu-id="ffb8e-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="ffb8e-107">在 Microsoft Intune 中新增適用於 iOS 與 iPadOS 裝置的 Wi-Fi 設定</span><span class="sxs-lookup"><span data-stu-id="ffb8e-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="ffb8e-108">在 Intune 中為 Windows 10 和更新版本裝置新增 Wi-Fi 設定</span><span class="sxs-lookup"><span data-stu-id="ffb8e-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="ffb8e-109">在 Intune 中為 Windows 裝置匯入 Wi-Fi 設定</span><span class="sxs-lookup"><span data-stu-id="ffb8e-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="ffb8e-110">**常見問題**</span><span class="sxs-lookup"><span data-stu-id="ffb8e-110">**Common Issues**</span></span>

<span data-ttu-id="ffb8e-111">**我要部署依賴於 Wi-Fi 設定檔中所指定的部署憑證的 Wi-Fi 設定檔。不過，組態設定檔顯示錯誤狀態。**</span><span class="sxs-lookup"><span data-stu-id="ffb8e-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="ffb8e-112">確定您的裝置已收到憑證。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="ffb8e-113">在 Intune 中，移至 [所有裝置]\*\*\*\*，然後選取裝置 > [裝置設定]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="ffb8e-114">確定所有預期的設定檔都已列出，並處於成功狀態。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="ffb8e-115">若是 Android 設定檔，如果您的憑證鏈結中有中繼憑證，請確認已將憑證部署到 Android 裝置。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="ffb8e-116">若要檢查憑證狀態，請移至 [裝置設定]\*\*\*\*  >  [設定檔]\*\*\*\*  >  [Android 中繼 CA]\*\*\*\*  >  [屬性]\*\*\*\*  >  [信任的憑證]\*\*\*\*。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="ffb8e-117">如果您持續看到錯誤，請檢閱程序和疑難排解小節。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="ffb8e-118">如需詳細資訊，請參閱[針對 SCEP 憑證設定檔搭配 Microsoft Intune 進行疑難排解的概觀](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="ffb8e-119">**我將 Wi-Fi 設定檔部署到裝置上。Intune 顯示它已成功完成，但裝置未連線至 Wi-Fi。**</span><span class="sxs-lookup"><span data-stu-id="ffb8e-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="ffb8e-120">成功狀態表示 Intune 已按照設定成功部署設定檔。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="ffb8e-121">不過，這些設定可能不符合您的網路和/或驗證需求。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="ffb8e-122">如需有關所嘗試連線的詳細資訊，請檢閱基礎結構和驗證服務 (Wi-Fi 存取點控制器和 NPS/RADIUS 伺服器) 中的記錄。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="ffb8e-123">您可能需要與您的網路基礎結構小組或第三方 Wi-Fi 廠商合作，來收集和檢閱記錄。</span><span class="sxs-lookup"><span data-stu-id="ffb8e-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>